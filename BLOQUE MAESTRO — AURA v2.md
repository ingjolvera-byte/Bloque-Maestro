================================================================
BLOQUE MAESTRO — AURA v2 (ESTADO ACTUAL COMPLETO)
================================================================

VERSIÓN:
AURA v2

FECHA:
2025-12-16

ESTADO GENERAL:
- Core: FUNCIONAL Y SELLADO
- UI v2: FUNCIONAL (Nova)
- Wake Word: IMPLEMENTACIÓN EN CURSO (FASE 11)
- LLM: FUNCIONAL (modo fallback)
- Arquitectura: RESPETADA
- Regla clave: SIEMPRE CÓDIGOS COMPLETOS (NO ADIVINANZAS)

================================================================
ESTRUCTURA DEL PROYECTO (REAL)
================================================================

AURA/
├─ core/
│  ├─ core.py
│  ├─ simple_responder.py
│  └─ stt_hook.py
│
├─ ui/
│  ├─ app.py
│  └─ ui.py
│
├─ voice/
│  ├─ stt.py
│  ├─ tts.py
│  └─ wakeword/
│     ├─ config.py
│     ├─ detector.py
│     └─ orchestrator.py
│
├─ models/
│  └─ vosk-es/
│
└─ main.py

================================================================
REGLAS DE PROYECTO (SELLADAS)
================================================================

1. El core NO se toca.
2. La UI NO contiene lógica.
3. El wake word vive SOLO en voice/.
4. La activación es EXTERNA al core.
5. Siempre se entregan ARCHIVOS COMPLETOS.
6. Nada de “busca”, “edita aquí”, “agrega esto”.
7. Todo es reversible.
8. Todo es local.
9. Texto plano siempre.

================================================================
ARCHIVO: voice/wakeword/config.py
================================================================

WAKE_WORD = "nova"

SAMPLE_RATE = 16000
CHANNELS = 1

LISTEN_WINDOW_SECONDS = 7
SILENCE_SECONDS = 2.0

================================================================
ARCHIVO: voice/wakeword/detector.py
================================================================

import json
import threading
import queue

import sounddevice as sd
from vosk import Model, KaldiRecognizer

from voice.wakeword.config import (
    WAKE_WORD,
    SAMPLE_RATE,
    CHANNELS,
)

MIC_DEVICE_ID = 7


class WakeWordDetector:
    def __init__(self, model_path: str):
        self.model = Model(model_path)
        self.recognizer = KaldiRecognizer(self.model, SAMPLE_RATE)
        self.recognizer.SetWords(True)

        self._running = False
        self._thread = None
        self._callback = None
        self._audio_q = queue.Queue()

    def on_detected(self, callback):
        self._callback = callback

    def start_listening(self):
        if self._running:
            return
        self._running = True
        self._thread = threading.Thread(target=self._run, daemon=True)
        self._thread.start()

    def stop_listening(self):
        self._running = False

    def _audio_callback(self, indata, frames, time_info, status):
        if status:
            return
        self._audio_q.put(bytes(indata))

    def _run(self):
        print("WakeWordDetector escuchando...")

        with sd.RawInputStream(
            samplerate=SAMPLE_RATE,
            blocksize=8000,
            dtype="int16",
            channels=CHANNELS,
            device=MIC_DEVICE_ID,
            callback=self._audio_callback,
        ):
            while self._running:
                try:
                    data = self._audio_q.get(timeout=0.5)
                except queue.Empty:
                    continue

                if self.recognizer.AcceptWaveform(data):
                    result = json.loads(self.recognizer.Result())
                    text = result.get("text", "").strip().lower()

                    print("VOSK TEXT:", text)

                    if WAKE_WORD in text.split() and self._callback:
                        print("WAKE WORD DETECTADO")
                        self._callback()
                        self.recognizer.Reset()

================================================================
ARCHIVO: voice/wakeword/orchestrator.py
================================================================

import threading

from voice.wakeword.detector import WakeWordDetector
from voice.stt import SpeechToText


class WakeWordOrchestrator:
    def __init__(self, model_path, core, ui_callback=None):
        self.core = core
        self.ui_callback = ui_callback
        self.detector = WakeWordDetector(model_path)
        self.stt = SpeechToText()

        self.detector.on_detected(self._on_wake)

    def start(self):
        self.detector.start_listening()

    def stop(self):
        self.detector.stop_listening()

    def _on_wake(self):
        if self.ui_callback:
            self.ui_callback("Escuchando")

        threading.Thread(target=self._listen_once, daemon=True).start()

    def _listen_once(self):
        text = self.stt.listen_once(timeout_seconds=7)
        if text:
            self.core.process_text(text)

        if self.ui_callback:
            self.ui_callback("Escuchando")

================================================================
ARCHIVO: ui/app.py
================================================================

import tkinter as tk
from tkinter import ttk


class AuraUI(tk.Tk):
    def __init__(self, core):
        super().__init__()
        self.core = core

        self.title("Nova")
        self.geometry("520x620")

        self.status_var = tk.StringVar(value="Escuchando")

        header = ttk.Frame(self, padding=10)
        header.pack(fill="x")

        ttk.Label(header, text="Nova", font=("Segoe UI", 18, "bold")).pack()
        ttk.Label(header, textvariable=self.status_var).pack()

        self.chat = tk.Text(self, state="disabled", wrap="word")
        self.chat.pack(expand=True, fill="both", padx=10, pady=10)

        input_frame = ttk.Frame(self)
        input_frame.pack(fill="x", padx=10, pady=10)

        self.entry = ttk.Entry(input_frame)
        self.entry.pack(side="left", expand=True, fill="x")
        self.entry.bind("<Return>", self._send)

        ttk.Button(input_frame, text="Enviar", command=self._send).pack(side="right")

    def _send(self, event=None):
        text = self.entry.get().strip()
        if not text:
            return

        self._append("Tú", text)
        self.entry.delete(0, "end")

        response = self.core.process_text(text)
        self._append("Nova", response)

    def _append(self, who, text):
        self.chat.configure(state="normal")
        self.chat.insert("end", f"{who}: {text}\n\n")
        self.chat.configure(state="disabled")
        self.chat.see("end")

================================================================
ARCHIVO: main.py
================================================================

from core.core import AuraCore
from ui.app import AuraUI
from voice.wakeword.orchestrator import WakeWordOrchestrator


def ui_state_update(state):
    app.status_var.set(state)


core = AuraCore()
app = AuraUI(core)

wake = WakeWordOrchestrator(
    model_path="models/vosk-es",
    core=core,
    ui_callback=ui_state_update
)

wake.start()
app.mainloop()

================================================================
ESTADO ACTUAL DE FASES
================================================================

FASE 9 — UI v2: CERRADA
FASE 11 — WAKE WORD:
- 11.1 → 11.6: DEFINIDAS
- 11.7 → 11.8: IMPLEMENTADAS
- 11.9: PRUEBAS EN CURSO

SIGUIENTE PASO EN NUEVO CHAT:
- Verificar detección estable
- Ajustar sensibilidad si hace falta
- Beep por audio real
- CIERRE FORMAL DE FASE 11

================================================================
FIN DEL BLOQUE MAESTRO
================================================================
