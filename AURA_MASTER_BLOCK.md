==================================================
BLOQUE MAESTRO — AURA V1
==================================================

ESTADO: CERRADO / CONGELADO
MODIFICACIONES: PROHIBIDAS
USO: REFERENCIA HISTÓRICA Y MEMORIA TÉCNICA

==================================================
DESCRIPCIÓN GENERAL
==================================================

AURA V1 corresponde a la primera iteración funcional
completa del asistente.

Esta versión contiene:
- Un core avanzado con manejo de estados
- STT funcional (varias aproximaciones)
- TTS funcional en Windows (SAPI)
- UI(s) operativas
- Sistema de memoria write-only
- Adaptador LLM local con fallback seguro
- Experimentos con wake word
- Scripts de prueba y runners auxiliares

V1 NO es un error.
V1 NO se elimina.
V1 NO se refactoriza.

V1 existe como referencia histórica y técnica
para entender decisiones futuras y evitar
repetir errores.

==================================================
ARQUITECTURA GENERAL V1
==================================================

- Arquitectura evolutiva
- Múltiples flujos coexistiendo
- Código experimental y estable mezclado
- Doble UI
- STT y wakeword en varias formas
- LLM encapsulado pero presente
- Memoria persistente básica

==================================================
CÓDIGOS FUNCIONALES CLAVE (REFERENCIA)
==================================================

--------------------------------------------------
CORE (REFERENCIA HISTÓRICA)
Ruta: core/core.py
--------------------------------------------------

class AuraCore:
    def __init__(self):
        self._state = "Escuchando"
        self._listeners = []

        self._tts = WindowsTTS()

        self._state_writer = AuraStateWriter()
        self.register_listener(self._state_writer.on_state_change)

        self._responder = AuraSimpleResponder(self)
        self._llm = AuraLLMAdapter()

        self._stt_hook = AuraSTTHook()
        self._stt_hook.enabled = True
        self._stt_hook.on_text_recognized = self._on_stt_text


--------------------------------------------------
LLM ADAPTER (REFERENCIA HISTÓRICA)
Ruta: models/llm_adapter.py
--------------------------------------------------

class AuraLLMAdapter:
    def request_response(self, input_text, context=None):
        if not self.enabled:
            return "No puedo responder a eso en este momento."
        # carga bajo demanda
        # timeout
        # fallback seguro


--------------------------------------------------
TTS WINDOWS (REFERENCIA HISTÓRICA)
Ruta: voice/windows_tts.py
--------------------------------------------------

class WindowsTTS:
    def speak(self, text: str):
        if not text:
            return
        self.voice.Speak(text)


==================================================
REGLAS DEL BLOQUE V1
==================================================

- Ningún archivo de V1 se modifica
- Ninguna decisión nueva se toma aquí
- No se empaqueta
- No se limpia
- Solo se documenta

==================================================
PROPÓSITO DEL BLOQUE V1
==================================================

- Memoria técnica
- Contexto histórico
- Referencia para debugging futuro
- Base conceptual de V2

==================================================
FIN BLOQUE MAESTRO — AURA V1
==================================================
