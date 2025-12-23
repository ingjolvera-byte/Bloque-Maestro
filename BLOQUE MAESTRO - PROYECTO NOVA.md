# BLOQUE MAESTRO — PROYECTO NOVA
Estado congelado y validado (incluye NOVA EXECUTOR)

## VISIÓN GENERAL

NOVA es una IA local (offline por defecto) diseñada para que el usuario dé órdenes en lenguaje natural y la IA ejecute acciones reales, sin exigir conocimientos técnicos, rutas, imports ni edición manual de código.

El usuario NO es constructor.  
El usuario es operador.

NOVA está compuesto por tres capas claras:

1. Interfaz (UI)  
2. Cerebro (NOVA Brain – decisión y lógica)  
3. Ejecutor (NOVA Executor – ejecución real y controlada)

El Executor NO es opcional conceptualmente, solo está **no integrado aún**.

## PRINCIPIOS FUNDAMENTALES (NO NEGOCIABLES)

1. El core no se rompe  
2. Nada se adivina  
3. Nada se toca parcialmente  
4. Nada se activa sin permiso explícito  
5. Todo cambio es aislado  
6. Un archivo por paso  
7. Código completo o nada  
8. El usuario manda, NOVA ejecuta  
9. Primero estabilidad, luego capacidades  
10. Offline primero, online solo bajo orden  

## REGLAS DE TRABAJO ACTIVAS

REGLA MAESTRA ACTIVA

NO se modifican archivos existentes del core.

Cualquier desarrollo nuevo:
- se hace en archivos nuevos
- no se importa
- no se ejecuta
- no se integra

hasta que el usuario lo autorice explícitamente.

Si una funcionalidad rompe esta regla, se cancela.

## ESTRUCTURA REAL DEL PROYECTO (CONFIRMADA Y FUTURA)

Ruta base del proyecto:
D:\NOVA\

Estructura completa del sistema:

- NOVA_IA
  - nova_brain.py (CORE – ESTABLE)
  - system_actions.py (ACCIONES LÓGICAS – ESTABLE)
  - memory.py / memory_manager.py (MEMORIA – ESTABLE)
  - env (entorno virtual)
  - STATUS.md (estado congelado)
  - interfaz
    - ui_chat_nova.py (INTERFAZ – ESTABLE)

  - modules (MÓDULOS AISLADOS – NO INTEGRADOS)
    - hardware
      - detect.py
    - dependencies
      - installer.py
    - translate
      - engine.py
      - models
      - status.json
      - README.md
    - voice
      - tts.py
      - stt.py
      - config.json
      - README.md

  - NOVA_EXECUTOR (NO INTEGRADO – PIEZA CLAVE)
    - nova_executor.py
    - task_schema.json
    - policies.json
    - queue.json
    - state.json
    - logs
    - README.md

Ruta de trabajo del usuario (salida de proyectos):

- C:\Users\ingjo\OneDrive\Documentos
  - NOVA_Proyectos
    - App_YYYYMMDD_HHMMSS
    - Chatbot_YYYYMMDD_HHMMSS
    - Web_YYYYMMDD_HHMMSS

## RUTA DE TRABAJO DEL USUARIO (CRÍTICA)

Todos los proyectos creados por NOVA van ÚNICAMENTE en:

C:\Users\ingjo\OneDrive\Documentos\NOVA_Proyectos

Nunca en:
- Documents genérico
- D:\
- rutas relativas
- carpetas del sistema

Esta ruta es sagrada.

## ESTADO ACTUAL (CHECKPOINT)

Estado confirmado:
- Sistema funcional
- Rutas correctas
- Memoria conectada
- Interfaz usable
- Usuario en control
- Cambios congelados
- Executor definido pero no integrado

Este es un checkpoint válido.
Todo avance futuro parte desde aquí.

## FUNCIONALIDADES CONFIRMADAS (YA FUNCIONAN)

CREACIÓN DE SOFTWARE (G)

NOVA puede crear:
- Apps
- Chatbots
- Páginas web

Mediante órdenes naturales, sin pedir rutas ni detalles técnicos.

LECTURA Y EDICIÓN BÁSICA (H)

NOVA puede:
- Recibir archivos adjuntos
- Leerlos
- Analizarlos
- Proponer cambios
- Aplicarlos solo con confirmación explícita

EMPAQUETADO BÁSICO (F)

- Estructuras limpias
- Preparación para entrega
- No destructivo
- No toca nada fuera de Documentos

MEMORIA PERSISTENTE REAL (D)

- Guarda preferencias del usuario
- Guarda historial básico
- Guarda proyectos creados
- Persiste entre ejecuciones

## NOVA EXECUTOR — DEFINICIÓN FORMAL

NOVA EXECUTOR es el componente encargado de ejecutar acciones reales del sistema de forma segura y controlada.

El Executor:
- NO decide
- NO conversa
- NO improvisa
- SOLO ejecuta tareas permitidas

El Executor recibe tareas estructuradas (JSON) desde el Brain.

Flujo lógico previsto:
Usuario → UI → Brain → Tarea estructurada → Executor → Resultado → UI

## POLÍTICAS DEL EXECUTOR

El Executor trabaja únicamente con una allowlist explícita.

Permitido:
- Crear archivos y carpetas dentro de NOVA_Proyectos
- Leer y escribir solo en rutas autorizadas
- Empaquetar proyectos
- Instalar dependencias dentro del env
- Detectar hardware (solo lectura)

Bloqueado SIEMPRE:
- Sistema operativo
- Registro
- Program Files
- Windows
- Acciones destructivas
- Ejecución arbitraria

Todo lo no permitido se rechaza.

## FUNCIONALIDADES APROBADAS PERO AISLADAS

Estas capacidades se implementarán a través del Executor:

- Detección automática de hardware
- Instalación automática de dependencias
- Traducción offline
- Voz (hablar y escuchar)

Ninguna toca el core.

## TRADUCCIÓN OFFLINE — CONDICIONES ACEPTADAS

La traducción offline está aprobada únicamente bajo estas condiciones:

1. No toca nova_brain.py  
2. No se importa al arrancar  
3. No bloquea la interfaz  
4. Vive en módulo dedicado  
5. Se activa solo con orden explícita  
6. Dependencias solo con confirmación  
7. Modelos se descargan una vez  
8. Idioma inicial: Inglés → Español  
9. No traduce código sin permiso  
10. Si falla, no miente  
11. Se puede desactivar  

## VOZ (HABLAR Y ESCUCHAR)

La voz está aprobada como concepto, pero NO integrada.

- Dependencia aparte
- Control total del usuario
- Nunca automática

Estado actual:
VOZ CONGELADA

## FILOSOFÍA DE DISEÑO

NOVA no debe:
- adivinar
- asumir
- improvisar
- ejecutar sin permiso

NOVA debe:
- preguntar
- ejecutar exactamente
- confirmar
- fallar de forma visible
- mantenerse estable

## PRÓXIMOS PASOS (NO ACTIVOS)

A elección del usuario:
- Integrar NOVA EXECUTOR
- Software real guiado (G+)
- Edición avanzada (H+)
- Empaquetado avanzado (F+)
- Traducción offline
- Voz

Nada se inicia sin confirmación explícita.

## FRASE DE CONTROL

Si en algún momento se propone:
modifica este archivo existente

La respuesta correcta es:
NO. Bloque maestro activo.

FIN DEL BLOQUE MAESTRO  
Estado CONGELADO  
Documento oficial del proyecto NOVA (incluye NOVA EXECUTOR)
