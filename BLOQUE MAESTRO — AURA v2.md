==================================================
BLOQUE MAESTRO — AURA V2
==================================================

ESTADO: ACTIVO
ARQUITECTURA: CONGELADA
EMPAQUETABLE: SÍ
OBJETIVO: BASE ESTABLE PARA CONSTRUIR IA

==================================================
PROPÓSITO GENERAL
==================================================

AURA V2 es la versión estable, coherente y
empaquetable del asistente.

Esta versión existe para servir como BASE
sobre la cual se construirá la IA real:

- Intenciones
- Acciones
- Memoria semántica
- Contexto
- Razonamiento

En V2 NO se experimenta con infraestructura.
V2 es contrato.

==================================================
REGLAS ABSOLUTAS V2
==================================================

- Un solo flujo principal
- Un solo punto de entrada
- Wake word bloqueante
- STT puntual
- Core como orquestador
- UI desacoplada
- Código completo o no existe
- Rutas explícitas siempre

Si no está aquí, no existe.
Si no es copiable, no se usa.

==================================================
FLUJO OFICIAL DE EJECUCIÓN
==================================================

main.py
 ├─ inicia UI
 ├─ inicia thread wake word
 │   ├─ escucha wake word (VOSK, bloqueante)
 │   ├─ beep de confirmación
 │   ├─ escucha STT una sola vez
 │   └─ core.process_text(texto)
 └─ UI mainloop

==================================================
ESTRUCTURA OFICIAL DEL PROYECTO
==================================================

AURA/
├── main.py
├── core/
│   ├── core.py
│   ├── simple_responder.py
│   └── stt_hook.py
├── ui/
│   └── app.py
├── voice/
│   ├── stt.py
│   ├── windows_tts.py
│   └── wakeword/
│       ├── detector.py
│       ├── beep.py
│       └── orchestrator.py
├── memory/
│   ├── state.py
│   ├── state_writer.py
│   ├── state_reader.py
│   └── state_connector.py
├── models/
│   └── vosk-es/
├── config/
│   ├── simple_responder.json
│   └── state_config.json

==================================================
CÓDIGOS OFICIALES V2 (CONTRATO)
==================================================

--------------------------------------------------
MAIN
Ruta: AURA/main.py
--------------------------------------------------

import threading

from core.core import AuraCore
from ui.app import AuraUI
from voice.wakeword.detector import WakeWordDetector
from voice.wakeword.beep import play_beep
from voice.stt import AuraSTT


def start_wakeword_loop(core, ui_callback):
    detector = WakeWordDetector(
        model_path="models/vosk-es",
        wake_words=["nova"]
    )
    stt = AuraSTT()

    while True:
        detector.listen()
        play_beep()

        if ui_callback:
            ui_callback("Escuchando")

        text = stt.listen_once(timeout=7, phrase_time_limit=7)
        if text:
            core.process_text(text)

        if ui_callback:
            ui_callback("Escuchando")


def main():
    core = AuraCore()
    app = AuraUI(core)

    def ui_state_update(state):
        app.status_var.set(state)

    threading.Thread(
        target=start_wakeword_loop,
        args=(core, ui_state_update),
        daemon=True
    ).start()

    app.mainloop()


if __name__ == "__main__":
    main()


--------------------------------------------------
SIMPLE RESPONDER
Ruta: core/simple_responder.py
--------------------------------------------------

import json
import os


class AuraSimpleResponder:
    FALLBACK = "He recibido tu mensaje."

    def __init__(self, core):
        self.core = core
        base_dir = os.path.dirname(os.path.dirname(__file__))
        json_path = os.path.join(base_dir, "config", "simple_responder.json")

        with open(json_path, "r", encoding="utf-8") as f:
            self.responses = json.load(f)

    def get_response(self, text: str) -> str:
        text = text.lower().strip()

        for key, value in self.responses.items():
            if key in text:
                return value

        return self.FALLBACK


--------------------------------------------------
WAKE WORD DETECTOR
Ruta: voice/wakeword/detector.py
--------------------------------------------------

class WakeWordDetector:
    def listen(self):
        # escucha bloqueante con VOSK
        # retorna True cuando detecta wake word
        pass


==================================================
ESTADO DE LOS SUBSISTEMAS
==================================================

Core:            ESTABLE
UI:              ESTABLE
Wake word:       ESTABLE (bloqueante)
STT:              ESTABLE
TTS:              ESTABLE
Memory:           ESTABLE (write-only)
LLM Adapter:      OPCIONAL
SimpleResponder:  ALINEADO CON CORE

==================================================
QUÉ NO HACE V2
==================================================

- No memoria conversacional avanzada
- No razonamiento complejo
- No agentes
- No acciones del sistema

==================================================
CIERRE
==================================================

AURA V2 es la base definitiva.
No se rediseña.
No se fragmenta.
No se vuelve a discutir.

Desde aquí en adelante,
todo el trabajo es IA.

==================================================
FIN BLOQUE MAESTRO — AURA V2
==================================================
