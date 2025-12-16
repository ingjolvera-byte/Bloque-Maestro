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
ANEXO — FASE 5.1: DEFINICIÓN DE MODELO LLM Y POLÍTICA DE USO
================================================================

FECHA: 2025-12-15

CONTEXTO:
Este anexo desarrolla la FASE 5 ya abierta, definiendo el marco exacto
en el que un MODELO LLM puede existir dentro de AURA.

TIPO DE MODELO PERMITIDO:
- Modelo de lenguaje LOCAL
- Ejecución OFFLINE
- Sin dependencias de servicios externos
- Compatible con ejecución controlada por proceso

MODELOS OBJETIVO (NO EXCLUSIVOS):
- Familia LLaMA (llama3)
- Familia Phi (phi3)

La elección final del modelo:
- NO altera la arquitectura
- NO altera el rol del LLM
- NO altera el control del core

ROL FUNCIONAL DEL MODELO:
El LLM se limita a:
- Recibir texto
- Generar texto
- Responder bajo contexto entregado

El LLM NO:
- Mantiene estado propio persistente
- Decide acciones
- Controla flujo
- Accede a hardware, sistema o red
- Interactúa directamente con el usuario

POLÍTICA DE INVOCACIÓN:
- El LLM solo puede ser invocado por el core
- La invocación es explícita
- No existe escucha continua del LLM
- Cada llamada es independiente

POLÍTICA DE CONTEXTO:
- El contexto enviado al LLM es mínimo
- Determinado únicamente por el core
- No existe memoria implícita entre llamadas
- El core puede enviar contexto vacío

POLÍTICA DE RESPUESTA:
- La respuesta del LLM es texto plano
- El core decide si se usa, filtra o descarta
- El LLM no habla directamente (TTS siempre controlado por el core)

PROHIBICIONES ABSOLUTAS:
- No streaming directo al usuario
- No ejecución de código generado
- No auto-llamadas
- No loops autónomos
- No escalamiento de privilegios

ESTADO:
Marco definido.
Sin implementación.
Sin integración.

FASE 5.1 DEFINIDA.

================================================================
ANEXO — FASE 5.2: DISEÑO DEL ADAPTADOR LLM (INTERFAZ)
================================================================

FECHA: 2025-12-15

OBJETIVO:
Definir la INTERFAZ FORMAL entre el core de AURA y el subsistema LLM,
sin implementar lógica, sin elegir librerías, sin escribir código.

PRINCIPIO FUNDAMENTAL:
El LLM NO se integra directamente al core.
La comunicación se realiza EXCLUSIVAMENTE a través de un ADAPTADOR.

ROL DEL ADAPTADOR LLM:
El adaptador actúa como:
- Punto único de entrada al LLM
- Capa de aislamiento
- Filtro de seguridad
- Traductor de contexto

El adaptador NO:
- Decide cuándo llamar al LLM
- Mantiene memoria persistente
- Ejecuta acciones
- Controla TTS o STT

RESPONSABILIDADES DEL ADAPTADOR:
- Recibir texto y contexto desde el core
- Enviar solicitud al modelo LLM
- Recibir respuesta textual
- Devolver texto al core sin modificarlo

INTERFAZ LÓGICA DEFINIDA:
El adaptador deberá exponer, como mínimo, una operación conceptual:

- request_response(input_text, context) → output_text

Donde:
- input_text: texto del usuario
- context: información opcional entregada por el core
- output_text: texto generado por el LLM

GESTIÓN DE CONTEXTO:
- El adaptador NO decide contexto
- El core construye y entrega el contexto
- El adaptador solo lo transmite

GESTIÓN DE ERRORES:
- Errores del LLM no se propagan al usuario
- El adaptador devuelve fallos controlados al core
- El core decide respuesta alternativa

POLÍTICA DE TIEMPO:
- Cada llamada al LLM es sincrónica y finita
- No se permiten ejecuciones indefinidas
- El core mantiene control temporal

UBICACIÓN EN LA ARQUITECTURA:
- El adaptador reside fuera del core
- Forma parte del subsistema de modelos
- Es reemplazable sin afectar al sistema

PROHIBICIONES:
- El adaptador no llama al core
- El adaptador no mantiene estado conversacional
- El adaptador no habla
- El adaptador no escucha

ESTADO:
Diseño aprobado.
Interfaz definida.
Implementación pendiente.

FASE 5.2 DEFINIDA.

================================================================
ANEXO — FASE 5.3: DISEÑO DEL FLUJO CORE → LLM → CORE
================================================================

FECHA: 2025-12-15

OBJETIVO:
Definir el FLUJO EXACTO de interacción entre el core de AURA y el LLM,
garantizando control total, previsibilidad y ausencia de autonomía.

PRINCIPIO FUNDAMENTAL:
El core es el ORQUESTADOR ABSOLUTO.
El LLM es un RECURSO INVOCADO, nunca un agente activo.

FLUJO GENERAL DEFINIDO:

1. Entrada de usuario
   - Origen: STT
   - El texto llega al core
   - El core valida el estado del sistema

2. Decisión de invocación
   - El core evalúa si el texto:
     - puede resolverse por reglas (Fase 4)
     - requiere procesamiento LLM (Fase 5)
   - Esta decisión es determinista y explícita

3. Preparación de contexto
   - El core construye el contexto
   - El contexto es:
     - mínimo
     - controlado
     - temporal
   - No existe contexto implícito

4. Llamada al adaptador LLM
   - El core invoca al ADAPTADOR
   - Envía:
     - texto del usuario
     - contexto preparado
   - El core queda a la espera

5. Procesamiento LLM
   - El LLM genera una respuesta textual
   - No ejecuta acciones
   - No modifica estado
   - No mantiene memoria

6. Retorno de respuesta
   - El adaptador devuelve texto plano al core
   - Errores se devuelven como estado controlado

7. Validación por el core
   - El core decide:
     - usar la respuesta
     - filtrar la respuesta
     - descartar la respuesta
   - El LLM no tiene decisión final

8. Salida al usuario
   - Si se acepta la respuesta:
     - el core la envía a TTS
   - Si se descarta:
     - el core responde con fallback controlado

GESTIÓN DE ESTADOS:
Durante este flujo:
- Escuchando → Procesando → Respondiendo → Escuchando
- El LLM NO altera estados
- El core mantiene coherencia del ciclo

GESTIÓN DE FALLOS:
- Fallo del LLM NO bloquea el sistema
- El core vuelve a estado estable
- Se emite respuesta neutra si es necesario

PROHIBICIONES ABSOLUTAS:
- El LLM no inicia flujo
- El LLM no llama al core
- El LLM no mantiene loops
- El LLM no accede a otros subsistemas

ESTADO:
Flujo definido.
Control garantizado.
Implementación pendiente.

FASE 5.3 DEFINIDA.

================================================================
ANEXO — FASE 5.4: CRITERIOS DE SEGURIDAD Y FALLBACK DEL LLM
================================================================

FECHA: 2025-12-15

OBJETIVO:
Definir los MECANISMOS DE SEGURIDAD, CONTENCIÓN y RESPUESTA AL FALLO
en la integración del LLM, garantizando que AURA nunca pierda control,
estabilidad ni autoridad del core.

PRINCIPIO FUNDAMENTAL:
El LLM es potencialmente falible.
El sistema debe permanecer estable incluso si el LLM:
- falla
- se bloquea
- responde incoherentemente
- no responde

TIPOS DE FALLO CONTEMPLADOS:

1. FALLO DE EJECUCIÓN
   - El LLM no responde
   - El proceso se detiene
   - Tiempo de espera excedido

2. FALLO DE CONTENIDO
   - Respuesta vacía
   - Respuesta incoherente
   - Respuesta irrelevante

3. FALLO DE INTEGRIDAD
   - Respuesta fuera de contexto
   - Respuesta no deseada
   - Respuesta incompatible con estado del sistema

POLÍTICA GENERAL DE SEGURIDAD:
- Ningún fallo del LLM puede bloquear el core
- Ningún fallo del LLM puede romper el ciclo de estados
- Ningún fallo del LLM puede propagarse al usuario como error técnico

MECANISMO DE FALLBACK:
Ante cualquier fallo del LLM:
- El core descarta la respuesta
- El core retorna a estado estable
- El core emite una respuesta neutra predefinida

RESPUESTA NEUTRA DE FALLBACK (CONCEPTUAL):
Ejemplos válidos:
- “No puedo responder a eso en este momento.”
- “He tenido un problema procesando la respuesta.”
- “Intentemos de nuevo.”

(La frase exacta será definida en implementación futura.)

CONTROL DE TIEMPO:
- Toda llamada al LLM tiene tiempo máximo finito
- El core puede cancelar la espera
- No se permiten bloqueos indefinidos

AUDITORÍA Y VISIBILIDAD:
- El core puede registrar internamente que ocurrió un fallo
- No se expone información técnica al usuario
- El sistema mantiene comportamiento predecible

PROHIBICIONES:
- El LLM no gestiona sus propios errores
- El LLM no decide fallback
- El LLM no reintenta automáticamente
- El LLM no ajusta su propio contexto

ESTADO:
Criterios definidos.
Riesgo controlado.
Implementación pendiente.

FASE 5.4 DEFINIDA.

================================================================
ANEXO — FASE 5.5: MODO DE ACTIVACIÓN DEL LLM (CUÁNDO SÍ / CUÁNDO NO)
================================================================

FECHA: 2025-12-15

OBJETIVO:
Definir de forma explícita y no ambigua CUÁNDO el core de AURA
está autorizado a invocar el LLM y CUÁNDO está prohibido hacerlo.

PRINCIPIO FUNDAMENTAL:
El LLM NO es la respuesta por defecto.
El LLM es un recurso excepcional, no primario.

CRITERIO GENERAL DE ACTIVACIÓN:
El LLM solo puede ser invocado cuando:
- Las reglas deterministas (Fase 4) no resuelven la entrada
- El texto del usuario requiere generación lingüística flexible
- El core determina explícitamente que el LLM es necesario

CRITERIOS EXPLÍCITOS DE NO ACTIVACIÓN:
El core NO debe invocar el LLM cuando:
- La entrada coincide con reglas simples conocidas
- La respuesta puede resolverse con datos del sistema
- El estado del sistema no es estable
- El sistema está en modo degradado o fallback
- La entrada es vacía, ruido o inválida

MODO DE DECISIÓN:
- La decisión de invocar LLM es determinista
- No existe auto-evaluación del LLM
- El core ejecuta la decisión, no el modelo

ORDEN DE PRIORIDAD DE RESPUESTA:
1. Respuestas internas deterministas (Fase 4)
2. Respuestas dinámicas del sistema
3. LLM (solo si lo anterior falla)

REVERSIBILIDAD:
- El core puede desactivar completamente el LLM
- El sistema debe seguir funcionando sin LLM
- No existe dependencia dura del LLM

VISIBILIDAD DE ACTIVACIÓN:
- El usuario no necesita saber si se usó LLM
- El comportamiento externo debe ser coherente
- No se expone complejidad interna

PROHIBICIONES ABSOLUTAS:
- El LLM no decide cuándo activarse
- El LLM no se auto-invoca
- El LLM no se usa como fallback primario
- El LLM no se usa para lógica de control

ESTADO:
Modo de activación definido.
Control garantizado.
Implementación pendiente.

FASE 5.5 DEFINIDA.

================================================================
ANEXO — FASE 5.6: PREPARACIÓN PARA IMPLEMENTACIÓN (CHECKLIST)
================================================================

FECHA: 2025-12-15

OBJETIVO:
Establecer las CONDICIONES NECESARIAS Y SUFICIENTES para autorizar
el paso desde DISEÑO a IMPLEMENTACIÓN del LLM en AURA.

Este anexo actúa como PUERTA DE CONTROL.
Sin cumplir este checklist, NO se escribe código.

CONDICIONES TÉCNICAS PREVIAS (OBLIGATORIAS):

- Arquitectura de Fase 5 completamente definida
- Rol del LLM claramente delimitado
- Adaptador LLM diseñado y aislado
- Flujo core → LLM → core definido
- Criterios de seguridad y fallback definidos
- Modo de activación del LLM definido
- Reversibilidad garantizada
- Sistema funcional sin LLM

CONDICIONES DE CONTROL:

- El core mantiene autoridad absoluta
- El LLM es invocable, no residente
- No existe dependencia dura del LLM
- El sistema puede operar con LLM deshabilitado
- El fallo del LLM no degrada el sistema

CONDICIONES DE IMPLEMENTACIÓN:

Antes de escribir código:
- Se define el primer archivo a crear
- Se define el primer archivo a modificar
- Se confirma que toda modificación será entregada COMPLETA
- Se confirma que no se romperá código congelado
- Se confirma que la implementación será incremental

CRITERIO DE AUTORIZACIÓN:

La implementación del LLM SOLO puede comenzar cuando:
- Todas las fases 5.1 → 5.6 estén definidas
- El usuario ordene explícitamente iniciar implementación
- El primer paso técnico sea mínimo, reversible y aislado

PROHIBICIONES EXPLÍCITAS:

- No se implementa “por probar”
- No se conecta el LLM directamente al core
- No se introduce IA fuera del marco definido
- No se adelantan capacidades futuras

ESTADO:

Checklist completo.
Condiciones claras.
Sistema autorizado para IMPLEMENTACIÓN
solo bajo orden explícita del usuario.

FASE 5.6 DEFINIDA.

================================================================
ANEXO — CIERRE DE FASE 5 (DUMMY): INTEGRACIÓN LLM SIMULADA
================================================================

FECHA DE CIERRE: 2025-12-15

FASE CERRADA:
FASE 5 — INTEGRACIÓN DE MODELO IA (LLM) — MODO DUMMY

ALCANCE DEL CIERRE:
La Fase 5 queda cerrada en su modalidad DUMMY tras haberse cumplido
de forma completa y verificable los siguientes hitos:

- Diseño completo de la Fase 5 (5.1 → 5.6)
- Definición del rol, límites y prohibiciones del LLM
- Diseño del adaptador LLM como capa aislada
- Implementación del adaptador LLM en modo DUMMY
- Respuesta simulada controlada del LLM
- Integración del adaptador con el core
- Decisión controlada del core:
  - prioridad a reglas deterministas (Fase 4)
  - escalado al LLM solo cuando corresponde
- Flujo completo validado:
  STT → core → adaptador LLM → core → TTS
- Ciclo de estados intacto y estable
- Sistema completamente funcional sin IA real

ESTADO DEL LLM EN ESTE CIERRE:
- LLM REAL: NO INTEGRADO
- LLM DUMMY: ACTIVO Y CONTROLADO
- Dependencia del LLM: NULA
- Reversibilidad: TOTAL

GARANTÍAS TRAS EL CIERRE:
- El core mantiene autoridad absoluta
- El sistema no depende del LLM
- El fallo del LLM no degrada AURA
- No existe deuda técnica
- La arquitectura queda preparada para LLM real

PROHIBICIONES A PARTIR DE ESTE CIERRE:
- No se amplía la lógica dummy
- No se simula inteligencia adicional
- No se introduce aprendizaje
- No se integra un LLM real fuera de una nueva fase

CONDICIÓN PARA AVANZAR:
La integración de un LLM REAL deberá realizarse en una
NUEVA FASE explícita, documentada y cerrada de forma independiente.

FASE 5 (DUMMY) CERRADA.

================================================================
AUTORIDAD FINAL
================================================================
El usuario manda.
El asistente obedece.
Este archivo es la ÚNICA fuente de verdad.

FIN DEL BLOQUE MAESTRO
