BLOQUE MAESTRO V2 — AURA

ESTADO:
Diseño base. No implementación todavía.
V1 NO SE TOCA.
V2 es un reinicio limpio.

OBJETIVO:
Reconstruir AURA desde cero de forma estable, simple y empaquetable,
sin que el usuario tenga que adivinar, recordar o modificar código.

REGLAS ABSOLUTAS:
- Todo en minúsculas (archivos, carpetas, imports)
- Un archivo = una responsabilidad
- No se modifica código fuera de bloques completos entregados
- Si no está aquí, no existe
- Si no es copiable, no se usa
- V1 no se modifica bajo ninguna circunstancia

QUE HACE AURA V2:
- Inicia sin cerrarse
- Detecta wakeword con vosk
- Escucha voz
- Convierte audio a texto
- Responde con respuestas simples desde un json
- Muestra estado por consola
- Se puede empaquetar con PyInstaller (onedir)

QUE NO HACE TODAVÍA:
- IA compleja
- memoria
- razonamiento
- interfaz gráfica avanzada

ESTRUCTURA DEFINITIVA DE CARPETAS:

aura/
│
├── main.py
│
├── core/
│   ├── __init__.py
│   ├── core.py
│   └── simple_responder.py
│
├── voice/
│   ├── __init__.py
│   ├── listener.py
│   └── wakeword/
│       ├── __init__.py
│       └── detector.py
│
├── data/
│   └── simple_responses.json
│
├── models/
│   └── vosk-model-small-es/
│
├── requirements.txt
└── README.md

RESPONSABILIDAD DE ARCHIVOS:

main.py
- punto de entrada
- manejo de errores global
- NO contiene lógica

core/core.py
- orquesta el flujo general
- recibe texto
- llama al responder

core/simple_responder.py
- carga data/simple_responses.json
- devuelve respuestas simples
- no maneja voz

data/simple_responses.json
- respuestas estáticas
- editable sin tocar código

voice/listener.py
- graba audio
- convierte audio a texto
- no decide respuestas

voice/wakeword/detector.py
- detecta palabra clave con vosk
- devuelve true o false
- no imprime ni responde

DEPENDENCIAS (requirements.txt):
vosk
sounddevice
numpy

EMPAQUETADO:
- pensado desde el diseño
- uso de rutas relativas
- soporte para PyInstaller onedir
- inclusión explícita de models/

METODO DE TRABAJO:
- el usuario NO modifica código a mano
- el asistente entrega archivos completos
- uno por uno
- listos para pegar
- sin interpretación

ORDEN DE IMPLEMENTACIÓN:
1. main.py
2. core/core.py
3. core/simple_responder.py
4. data/simple_responses.json
5. voice/listener.py
6. voice/wakeword/detector.py
7. empaquetado

FRASE CLAVE:
Si no es copiable, no se hace.
Si no está en el bloque maestro, no existe.
