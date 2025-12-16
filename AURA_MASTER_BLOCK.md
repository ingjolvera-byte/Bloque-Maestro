PROYECTO: AURA
TIPO: BLOQUE MAESTRO ABSOLUTO
ESTADO: DEFINITIVO – APPEND-ONLY – NO INTERPRETABLE
FECHA CREACIÓN: 2025-12-13
ACTUALIZACIÓN: 2025-12-15

================================================================
PRINCIPIO FUNDAMENTAL
================================================================
El usuario NO programa.
El usuario NO entiende código.
El usuario NO toma decisiones técnicas.
El usuario NO completa fragmentos.
El usuario NO deduce cambios.

El asistente:
- recuerda todo lo definido
- no vuelve a pedir información ya definida
- no improvisa
- no reestructura
- no explica de más
- no divide entregas
- no corta código
- no entrega fragmentos de archivos existentes
- no obliga al usuario a inferir cambios
- no pregunta “qué quieres hacer ahora”
- NO entrega el Bloque Maestro en otro formato que no sea TEXTO PLANO

Si algo está definido aquí, NO se vuelve a preguntar.
Si un archivo es modificado, DEBE entregarse COMPLETO.

================================================================
REGLA ABSOLUTA DE ENTREGA DE CÓDIGO
================================================================
Cuando el asistente:
- modifique un archivo existente
- amplíe un archivo existente
- conecte un subsistema a un archivo existente

ENTONCES:
- DEBE entregar el archivo COMPLETO
- DEBE estar listo para copiar/pegar
- DEBE ser TEXTO PLANO
- DEBE ser UN SOLO BLOQUE
- DEBE poder subirse directo a GitHub
- ESTÁ PROHIBIDO entregar diffs, fragmentos o instrucciones parciales

El usuario nunca adivina.
El asistente siempre entrega completo.

================================================================
REGLA DE ENTREGA DEL BLOQUE MAESTRO
================================================================
Cada vez que el usuario solicite el Bloque Maestro:

- El asistente DEBE enviarlo COMPLETO.
- El asistente DEBE enviarlo en TEXTO PLANO.
- El asistente DEBE enviarlo en UN SOLO BLOQUE.
- El contenido DEBE estar listo para copiar/pegar en GitHub.
- Está prohibido enviar versiones parciales, resúmenes o explicaciones.

El incumplimiento invalida la entrega.

================================================================
DEFINICIÓN DE LA IA AURA
================================================================
AURA es una IA LOCAL, personal y empresarial.

AURA actúa como:
- asistente personal
- asistente empresarial
- agenda parlante
- apoyo creativo
- apoyo en desarrollo de software
- creadora de documentos empresariales
- protectora del sistema
- interfaz hombre–máquina avanzada

AURA NO es:
- chatbot
- app web
- demo
- proyecto académico
- curso de programación

================================================================
ESTADO ACTUAL DEPURADO DEL PROYECTO
================================================================
El proyecto AURA se encuentra en estado DEPURADO.

- Bloque Maestro clarificado y sellado.
- Solo lo funcional y repetible manda.
- No hay deuda técnica activa.

================================================================
DECISIÓN OPERATIVA ACTUAL
================================================================
STT (Escucha): STAND BY
TTS (Voz): ACTIVO – INTEGRADO AL CORE

- STT existe pero permanece aislado.
- TTS es subsistema estable.
- STT NO se modifica.

================================================================
INSTRUCCIÓN EXPLÍCITA PARA CONTINUIDAD
================================================================
- El asistente continúa según el ORDEN MÁS PRUDENTE.
- El asistente NO pregunta qué hacer.
- El asistente NO ofrece bifurcaciones.
- El asistente propone un único siguiente paso lógico.

================================================================
ESTRUCTURA DEFINITIVA (NOMBRES FIJOS)
================================================================

AURA/
├─ main.py
├─ core/
│  ├─ core.py
│  └─ state_hook.py
├─ ui/
│  └─ ui.py
├─ voice/
│  ├─ grabar.py
│  ├─ windows_tts.py
│  └─ voice.py
├─ memory/
│  ├─ state.py
│  ├─ state_reader.py
│  ├─ state_writer.py
│  └─ state_connector.py
├─ config/
│  ├─ config.json
│  └─ state_config.json

================================================================
PARTE B — REGISTRO DE AVANCES (APPEND-ONLY)
================================================================

[2025-12-15]
- TTS integrado al core.
- UI funcional.
- Memoria de estado implementada (write-only).
- Subsistema de memoria SELLADO.

================================================================
CÓDIGO FUNCIONAL REAL
================================================================

ARCHIVO: AURA/main.py
------------------------------------------------
from core.core import AuraCore
from ui.ui import AuraUI

def main():
    core = AuraCore()
    ui = AuraUI(core)
    ui.run()

if __name__ == "__main__":
    main()

------------------------------------------------
ARCHIVO: AURA/core/core.py
------------------------------------------------
from voice.windows_tts import WindowsTTS
from memory.state_writer import AuraStateWriter

class AuraCore:
    def __init__(self):
        self._state = "Escuchando"
        self._listeners = []
        self._tts = WindowsTTS()

        self._state_writer = AuraStateWriter()
        self.register_listener(self._state_writer.on_state_change)

    def get_status(self):
        return self._state

    def set_status(self, new_status):
        if new_status != self._state:
            self._state = new_status
            self._notify()
            self._speak_status(new_status)

    def _speak_status(self, status):
        frases = {
            "Escuchando": "Estoy escuchando.",
            "Procesando": "Procesando información.",
            "Respondiendo": "Aquí está mi respuesta."
        }
        texto = frases.get(status)
        if texto:
            self._tts.speak(texto)

    def register_listener(self, callback):
        if callback not in self._listeners:
            self._listeners.append(callback)

    def _notify(self):
        for callback in self._listeners:
            callback(self._state)

------------------------------------------------
ARCHIVO: AURA/ui/ui.py
------------------------------------------------
import tkinter as tk

class AuraUI:
    def __init__(self, core):
        self.core = core
        self.root = tk.Tk()
        self.root.title("AURA")
        self.root.geometry("600x400")
        self.root.configure(bg="#0a0f1e")

        self.status_var = tk.StringVar(value=self.core.get_status())
        self.core.register_listener(self._on_status_change)

        self._build_ui()
        self._demo_cycle()

    def _build_ui(self):
        title = tk.Label(self.root, text="AURA", fg="#00eaff", bg="#0a0f1e",
                         font=("Segoe UI", 28, "bold"))
        title.pack(pady=40)

        self.status_label = tk.Label(
            self.root,
            textvariable=self.status_var,
            fg="#ffffff",
            bg="#0a0f1e",
            font=("Segoe UI", 14)
        )
        self.status_label.pack(pady=20)

    def _on_status_change(self, new_status):
        self.status_var.set(f"Estado: {new_status}")

    def _demo_cycle(self):
        sequence = ["Escuchando", "Procesando", "Respondiendo"]
        current = self.core.get_status()
        next_state = sequence[(sequence.index(current) + 1) % len(sequence)]
        self.core.set_status(next_state)
        self.root.after(2000, self._demo_cycle)

    def run(self):
        self.root.mainloop()

------------------------------------------------
ARCHIVO: AURA/voice/windows_tts.py
------------------------------------------------
import win32com.client
import pythoncom
import threading

class WindowsTTS:
    def __init__(self):
        self._lock = threading.Lock()
        self._speaker = None

    def _init_sapi(self):
        pythoncom.CoInitialize()
        return win32com.client.Dispatch("SAPI.SpVoice")

    def speak(self, text):
        if not text:
            return
        with self._lock:
            if self._speaker is None:
                self._speaker = self._init_sapi()
            self._speaker.Speak(text)

================================================================
ANEXO — SELLADO DE SUBSISTEMA: MEMORIA DE ESTADO
================================================================

FECHA: 2025-12-15

- Escritura persistente: ACTIVA (write-only)
- Lectura: PREPARADA, NO ACTIVA
- Restauración: PROHIBIDA
- Modificación futura: SOLO por orden explícita del usuario
- Archivos completos obligatorios
- Append-only obligatorio

SUBSISTEMA SELLADO.

================================================================
AUTORIDAD FINAL
================================================================
El usuario manda.
El asistente obedece.
Este archivo es la ÚNICA fuente de verdad.

FIN DEL BLOQUE MAESTRO
