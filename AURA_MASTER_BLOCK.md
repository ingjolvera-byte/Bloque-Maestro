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
- El contenido DEBE estar listo para copiar/pegar directamente en GitHub.
- Está prohibido enviar versiones parciales, resúmenes, enlaces o explicaciones.

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

- Bloque Maestro clarificado y sellado por fases.
- Solo lo funcional y repetible manda.
- No hay deuda técnica activa.

================================================================
DECISIÓN OPERATIVA ACTUAL
================================================================
STT (Escucha): ACTIVO – INTEGRADO
TTS (Voz): ACTIVO – INTEGRADO AL CORE

- STT funcional y controlado.
- TTS subsistema estable.
- Ambos integrados sin IA.

================================================================
INSTRUCCIÓN EXPLÍCITA PARA CONTINUIDAD
================================================================
- El asistente continúa siempre según el ORDEN MÁS PRUDENTE.
- El asistente NO pregunta qué hacer.
- El asistente NO ofrece bifurcaciones.
- El asistente propone un único siguiente paso lógico cuando corresponde.

================================================================
ESTRUCTURA DEFINITIVA (NOMBRES FIJOS)
================================================================

AURA/
├─ main.py
├─ core/
│  ├─ core.py
│  ├─ simple_responder.py
│  ├─ stt_hook.py
│  └─ state_hook.py
├─ ui/
│  └─ ui.py
├─ voice/
│  ├─ stt.py
│  ├─ stt_bridge.py
│  ├─ windows_tts.py
│  └─ voice.py
├─ memory/
│  ├─ state.py
│  ├─ state_reader.py
│  ├─ state_writer.py
│  └─ state_connector.py
├─ config/
│  ├─ config.json
│  ├─ state_config.json
│  └─ simple_responses.json
└─ models/
   ├─ llama3/
   └─ phi3/

================================================================
PARTE B — REGISTRO DE FASES (APPEND-ONLY)
================================================================

FASE 1 — NÚCLEO OPERATIVO BÁSICO
ESTADO: CERRADA
- Arranque estable
- UI local
- Gestión de estados
- TTS integrado

FASE 2 — MEMORIA DE ESTADO
ESTADO: CERRADA / SELLADA
- Persistencia write-only
- Lectura preparada
- Restauración prohibida

FASE 3 — INTERACCIÓN BÁSICA VOZ ↔ CORE
ESTADO: CERRADA
- STT real
- Integración controlada
- Ciclo de estados completo
- Respuesta verbal mínima

FASE 4 — INTERACCIÓN CONVERSACIONAL SIMPLE
ESTADO: CERRADA
- Respuestas deterministas
- Respuestas por plantillas
- Respuestas dinámicas reales
- Sin IA
- Sin LLM
- Sin memoria conversacional

================================================================
ANEXO — CIERRE DE FASE 4
================================================================

FECHA: 2025-12-15

La Fase 4 queda formalmente cerrada.
Cualquier avance posterior pertenece a una nueva fase.

================================================================
ANEXO — APERTURA DE FASE 5: INTEGRACIÓN DE MODELO IA (LLM LOCAL)
================================================================

FECHA DE APERTURA: 2025-12-15

FASE ABIERTA:
FASE 5 — INTEGRACIÓN DE MODELO IA (LLM LOCAL)

OBJETIVO DE LA FASE:
Dotar a AURA de capacidad de procesamiento lingüístico avanzado mediante
un MODELO DE LENGUAJE LOCAL (LLM), manteniendo control total del sistema,
sin perder estabilidad, previsibilidad ni autoridad del usuario.

ROL DEL LLM EN AURA:
El LLM actúa EXCLUSIVAMENTE como:
- Motor de generación de lenguaje
- Intérprete semántico del texto recibido
- Asistente de razonamiento bajo demanda

El LLM NO es:
- Autoridad del sistema
- Tomador de decisiones finales
- Agente autónomo
- Sustituto del core
- Sustituto del usuario

UBICACIÓN ARQUITECTÓNICA:
- El LLM NO vive en el core
- El LLM se integra como SUBSISTEMA EXTERNO
- El core orquesta, el LLM responde
- El core siempre mantiene control del flujo

FLUJO CONTROLADO DE DATOS:
STT → core → (llamada explícita) → LLM → core → TTS

El LLM:
- NO accede directamente a STT
- NO accede directamente a TTS
- NO accede a sistema ni archivos
- NO persiste memoria por sí mismo

PROHIBICIONES EXPLÍCITAS EN ESTA FASE:
- No autonomía
- No ejecución de acciones
- No acceso directo al sistema
- No modificación de estado sin autorización del core
- No memoria propia persistente
- No aprendizaje fuera de sesión

PRINCIPIO DE CONTROL:
- El core decide CUÁNDO llamar al LLM
- El core decide QUÉ enviar al LLM
- El core decide SI usar la respuesta
- El core puede ignorar o descartar respuestas del LLM

CRITERIOS DE ÉXITO DE LA FASE 5:
La Fase 5 se considerará completada cuando:
- Un LLM local esté integrado funcionalmente
- El LLM genere respuestas coherentes bajo control del core
- No exista impacto negativo en estabilidad
- No exista deuda técnica
- El sistema siga siendo reversible y auditable

CONDICIÓN PARA AVANZAR:
Ninguna implementación técnica se realizará fuera del marco de este anexo.
Cualquier paso deberá respetar estrictamente lo aquí definido.

FASE 5 ABIERTA.

================================================================
AUTORIDAD FINAL
================================================================
El usuario manda.
El asistente obedece.
Este archivo es la ÚNICA fuente de verdad.

FIN DEL BLOQUE MAESTRO
