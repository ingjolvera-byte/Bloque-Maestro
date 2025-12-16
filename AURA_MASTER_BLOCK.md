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
ANEXO — APERTURA DE FASE 6: INTEGRACIÓN DE LLM REAL (LOCAL)
================================================================

FECHA DE APERTURA: 2025-12-15

FASE ABIERTA:
FASE 6 — INTEGRACIÓN DE MODELO LLM REAL (LOCAL)

CONTEXTO:
La Fase 5 (Dummy) ha sido cerrada con éxito.
El flujo, control y arquitectura han sido validados sin riesgo.
Esta fase introduce, por primera vez, un MODELO LLM REAL.

OBJETIVO DE LA FASE:
Sustituir el LLM DUMMY por un MODELO DE LENGUAJE LOCAL REAL,
manteniendo EXACTAMENTE el mismo flujo, control y arquitectura
validados en la Fase 5.

PRINCIPIO FUNDAMENTAL:
El LLM REAL debe comportarse, desde el core, de forma indistinguible
del LLM Dummy, salvo por la calidad de la respuesta.

Si el LLM REAL rompe el sistema,
el sistema está mal diseñado.
Este principio es vinculante.

ROL DEL LLM REAL:
- Generar texto coherente
- Procesar lenguaje natural
- Responder bajo demanda del core

EL LLM REAL NO:
- Decide flujo
- Decide acciones
- Accede al sistema
- Mantiene memoria propia
- Ejecuta código
- Controla TTS o STT

REQUISITOS DEL MODELO:
- Ejecución 100% local
- Sin dependencias cloud
- Control por proceso
- Arranque y parada explícitos
- Compatible con aislamiento del sistema

MODELOS CANDIDATOS:
- LLaMA (llama3)
- Phi (phi3)

(La elección concreta se realizará dentro de esta fase,
sin alterar arquitectura.)

CRITERIO DE SEGURIDAD:
- El sistema debe funcionar sin LLM
- El sistema debe recuperarse ante fallo del LLM
- El LLM es reemplazable sin modificar el core

CONDICIÓN DE ENTRADA A IMPLEMENTACIÓN:
No se escribirá código hasta:
- definir el método de carga del modelo
- definir el método de inferencia
- definir límites de recursos
- definir mecanismo de apagado seguro

ESTADO:
Fase abierta.
Arquitectura heredada de Fase 5.
Implementación pendiente.

FASE 6 ABIERTA.

================================================================
ANEXO — FASE 6.1: SELECCIÓN Y CRITERIOS DEL MODELO LLM REAL
================================================================

FECHA: 2025-12-15

OBJETIVO:
Definir los CRITERIOS FORMALES para la selección de un MODELO LLM REAL
que será integrado en AURA, sin realizar aún ninguna instalación
ni implementación técnica.

PRINCIPIO FUNDAMENTAL:
El modelo se adapta a la arquitectura.
La arquitectura NO se adapta al modelo.

CRITERIOS OBLIGATORIOS DEL MODELO:

1. EJECUCIÓN LOCAL
   - El modelo debe ejecutarse completamente offline
   - No se permiten llamadas a servicios externos
   - No dependencia de APIs cloud

2. CONTROL DE PROCESO
   - El modelo debe poder iniciarse y detenerse explícitamente
   - El core mantiene control del ciclo de vida
   - No procesos persistentes ocultos

3. AISLAMIENTO
   - El modelo no accede al sistema de archivos
   - El modelo no accede a red
   - El modelo no ejecuta código

4. INTERFAZ SIMPLE
   - Entrada: texto plano + contexto controlado
   - Salida: texto plano
   - Sin efectos colaterales

5. RECURSOS
   - Uso de CPU/GPU controlable
   - Uso de memoria predecible
   - Capaz de ejecutarse en hardware local razonable

MODELOS CANDIDATOS ACEPTADOS:

- LLaMA 3 (familia llama3)
- Phi 3 (familia phi3)

La elección entre ellos:
- No altera el rol del LLM
- No altera el flujo definido
- No altera el core

CRITERIOS DE DESCARTE:
Un modelo será descartado si:
- Requiere conexión externa
- Introduce dependencia no controlable
- No permite control de recursos
- Impone arquitectura propia

CRITERIO DE ÉXITO DE ESTA SUBFASE:
- Modelo elegido explícitamente
- Justificación basada en los criterios anteriores
- Sin implementación aún

ESTADO:
Criterios definidos.
Modelo aún no seleccionado.
Implementación pendiente.

FASE 6.1 DEFINIDA.

================================================================
ANEXO — FASE 6.2: DEFINICIÓN DEL MÉTODO DE CARGA DEL MODELO LLM
================================================================

FECHA: 2025-12-15

OBJETIVO:
Definir el MÉTODO DE CARGA del MODELO LLM REAL dentro de AURA,
garantizando control del ciclo de vida, aislamiento y reversibilidad,
antes de escribir cualquier código.

PRINCIPIO FUNDAMENTAL:
El modelo se carga BAJO DEMANDA y BAJO CONTROL.
El modelo no vive permanentemente en memoria sin autorización explícita.

MODO DE CARGA DEFINIDO:

- El LLM se carga como PROCESO CONTROLADO
- El inicio del modelo es explícito
- El apagado del modelo es explícito
- No se permiten autoarranques implícitos

CONTROL DEL CICLO DE VIDA:

El sistema debe poder:
- Inicializar el modelo
- Confirmar que el modelo está listo
- Ejecutar inferencias
- Detener el modelo limpiamente
- Liberar recursos

El core:
- Decide cuándo cargar el modelo
- Decide cuándo descargarlo
- Puede operar sin el modelo cargado

AISLAMIENTO DE CARGA:

- El modelo no se carga dentro del core
- El modelo se carga a través del ADAPTADOR LLM
- El core no conoce detalles internos de carga

GESTIÓN DE ERRORES DE CARGA:

Si el modelo:
- No carga
- Falla al inicializar
- Consume recursos excesivos

ENTONCES:
- El adaptador informa fallo al core
- El core mantiene funcionamiento normal
- Se activa modo fallback

POLÍTICA DE REINTENTO:

- No existen reintentos automáticos
- El core decide si reintentar
- Cada intento es explícito y controlado

CRITERIO DE ÉXITO DE ESTA SUBFASE:

- Método de carga definido conceptualmente
- Control del ciclo de vida garantizado
- Sin dependencia dura del modelo

ESTADO:
Método de carga definido.
Implementación pendiente.

FASE 6.2 DEFINIDA.

================================================================
ANEXO — FASE 6.3: DEFINICIÓN DEL MÉTODO DE INFERENCIA DEL LLM
================================================================

FECHA: 2025-12-15

OBJETIVO:
Definir el MÉTODO DE INFERENCIA mediante el cual el core de AURA
solicita una respuesta al MODELO LLM REAL, garantizando control,
previsibilidad y ausencia de efectos colaterales.

PRINCIPIO FUNDAMENTAL:
La inferencia es una OPERACIÓN PUNTUAL.
No existe ejecución continua ni streaming no controlado.

MODO DE INFERENCIA DEFINIDO:

- La inferencia se ejecuta bajo demanda
- Cada inferencia es independiente
- No existe estado interno persistente entre inferencias
- No existe inferencia en segundo plano

INTERFAZ DE INFERENCIA (CONCEPTUAL):

- Entrada:
  - texto del usuario
  - contexto temporal controlado por el core
- Salida:
  - texto plano generado por el modelo

No se admiten:
- respuestas parciales
- streaming directo al usuario
- callbacks autónomos

CONTROL TEMPORAL:

- Cada inferencia tiene tiempo máximo finito
- El core puede cancelar la espera
- El bloqueo indefinido está prohibido

CONTROL DE RECURSOS:

- Uso de CPU/GPU acotado
- Uso de memoria acotado
- Sin crecimiento acumulativo entre llamadas

GESTIÓN DE ERRORES DE INFERENCIA:

Si durante la inferencia ocurre:
- timeout
- error del modelo
- respuesta vacía o inválida

ENTONCES:
- El adaptador devuelve fallo controlado
- El core activa fallback definido en Fase 5.4
- El sistema vuelve a estado estable

AISLAMIENTO:

- El modelo no conoce el estado del sistema
- El modelo no conoce decisiones del core
- El modelo no accede a otros subsistemas

CRITERIO DE ÉXITO DE ESTA SUBFASE:

- Método de inferencia claramente definido
- Control temporal garantizado
- Fallos contenidos
- Sistema estable ante error

ESTADO:
Método de inferencia definido.
Implementación pendiente.

FASE 6.3 DEFINIDA.

================================================================
ANEXO — FASE 6.4: LÍMITES DE CONTEXTO Y PROMPTING DEL LLM
================================================================

FECHA: 2025-12-15

OBJETIVO:
Definir de forma estricta los LÍMITES DEL CONTEXTO y las reglas de
PROMPTING utilizadas al invocar el LLM, garantizando seguridad,
previsibilidad y control del comportamiento.

PRINCIPIO FUNDAMENTAL:
El LLM solo ve lo que el core decide mostrarle.
No existe contexto implícito ni memoria oculta.

DEFINICIÓN DE CONTEXTO:

El contexto enviado al LLM puede incluir:
- Texto actual del usuario
- Información explícita y puntual del sistema
- Instrucciones de rol definidas por el core

El contexto NO puede incluir:
- Historial completo de conversaciones
- Estado interno sensible del sistema
- Información privada no autorizada
- Rutas de archivos, comandos o credenciales

LÍMITES DE CONTEXTO:

- El contexto es TEMPORAL
- Se construye por solicitud
- Se descarta tras la inferencia
- No se reutiliza automáticamente

POLÍTICA DE PROMPTING:

- El prompt es generado exclusivamente por el core
- El usuario no controla directamente el prompt
- El LLM no modifica su propio prompt
- No existe prompt autoevolutivo

INSTRUCCIONES DE ROL:

El core puede incluir instrucciones como:
- “Responde de forma clara y concisa”
- “No tomes decisiones”
- “No ejecutes acciones”
- “Limítate a responder texto”

Estas instrucciones:
- Son estáticas o controladas
- No se aprenden
- No se modifican por el LLM

CONTROL DE LONGITUD:

- Longitud máxima de entrada definida
- Longitud máxima de salida definida
- El core puede truncar entradas
- El core puede truncar salidas

PROHIBICIONES ABSOLUTAS:

- No se envían instrucciones para auto-modificación
- No se envían instrucciones de evasión de control
- No se envían instrucciones de persistencia
- No se envían instrucciones para ejecutar código

CRITERIO DE ÉXITO DE ESTA SUBFASE:

- Contexto claramente delimitado
- Prompting controlado
- Riesgo de comportamiento no deseado minimizado

ESTADO:
Límites definidos.
Prompting controlado.
Implementación pendiente.

FASE 6.4 DEFINIDA.

================================================================
ANEXO — FASE 6.5: LÍMITES DE RECURSOS Y RENDIMIENTO DEL LLM
================================================================

FECHA: 2025-12-15

OBJETIVO:
Definir los LÍMITES DE CONSUMO DE RECURSOS y los CRITERIOS DE RENDIMIENTO
del MODELO LLM REAL, garantizando que AURA no degrade el sistema
ni comprometa la experiencia del usuario.

PRINCIPIO FUNDAMENTAL:
El LLM es un recurso costoso y secundario.
El sistema tiene prioridad absoluta sobre el modelo.

RECURSOS CONTROLADOS:

- CPU
- GPU (si aplica)
- Memoria RAM
- Tiempo de ejecución

LÍMITES GENERALES:

- El uso de CPU del LLM debe ser acotado
- El uso de memoria debe ser predecible
- El modelo no puede consumir recursos ilimitadamente
- El sistema debe seguir siendo usable durante inferencia

POLÍTICA DE MEMORIA:

- Memoria máxima permitida definida explícitamente
- Sin crecimiento acumulativo entre inferencias
- Liberación de memoria tras descarga del modelo

POLÍTICA DE TIEMPO:

- Tiempo máximo por inferencia definido
- El core puede abortar inferencias lentas
- No se permiten inferencias prolongadas indefinidamente

POLÍTICA DE PRIORIDAD:

- El sistema operativo tiene prioridad
- El core tiene prioridad
- El LLM siempre es de prioridad inferior

GESTIÓN DE SOBRECARGA:

Si el sistema detecta:
- consumo excesivo
- latencia elevada
- degradación perceptible

ENTONCES:
- El core desactiva el LLM
- Se retorna a respuestas deterministas
- Se informa internamente del evento

MODOS DE OPERACIÓN:

- Modo normal: LLM habilitado bajo límites
- Modo degradado: LLM deshabilitado
- Modo recuperación: LLM no disponible temporalmente

CRITERIO DE ÉXITO DE ESTA SUBFASE:

- Recursos claramente acotados
- Rendimiento aceptable definido
- Capacidad de desactivar LLM sin impacto funcional

ESTADO:
Límites de recursos definidos.
Rendimiento controlado.
Implementación pendiente.

FASE 6.5 DEFINIDA.

================================================================
ANEXO — FASE 6.6: CHECKLIST DE ENTRADA A IMPLEMENTACIÓN DEL LLM REAL
================================================================

FECHA: 2025-12-15

OBJETIVO:
Establecer la PUERTA FINAL DE CONTROL antes de autorizar la
IMPLEMENTACIÓN DEL LLM REAL en AURA.

Sin cumplir este checklist, NO se escribe código.

PRINCIPIO FUNDAMENTAL:
La implementación solo ocurre cuando el diseño está completo,
el riesgo está acotado y la reversibilidad está garantizada.

CHECKLIST OBLIGATORIO (TODOS DEBEN CUMPLIRSE):

ARQUITECTURA
- Fase 6 definida y abierta
- Subfases 6.1 → 6.5 definidas
- Arquitectura heredada de Fase 5 respetada
- Adaptador LLM definido como único punto de acceso

CONTROL
- El core mantiene autoridad absoluta
- El LLM es invocado, no residente
- El sistema funciona sin LLM
- El LLM puede desactivarse en cualquier momento

SEGURIDAD
- Flujo core → LLM → core definido
- Fallback definido y probado conceptualmente
- El LLM no accede a sistema, red ni archivos
- No existe ejecución de código generado

RECURSOS
- Límites de CPU definidos
- Límites de memoria definidos
- Límites de tiempo definidos
- Capacidad de abortar inferencias

PROMPTING Y CONTEXTO
- Contexto mínimo y temporal
- Prompt controlado por el core
- Sin memoria implícita
- Sin prompt autoevolutivo

IMPLEMENTACIÓN
- Primer archivo a modificar identificado
- Primer archivo a crear identificado
- Entrega de archivos completos garantizada
- Implementación incremental y reversible

AUTORIZACIÓN
La implementación del LLM REAL SOLO puede comenzar si:
- Este checklist está completo
- El usuario ordena explícitamente “Iniciar implementación LLM real”
- El primer paso técnico es mínimo y aislado

ESTADO:
Checklist completo.
Puerta de implementación definida.
Implementación BLOQUEADA hasta orden explícita.

FASE 6.6 DEFINIDA.

================================================================
ANEXO — CIERRE DE FASE 6: INTEGRACIÓN DE LLM REAL (DISEÑO + BASE)
================================================================

FECHA DE CIERRE: 2025-12-15

FASE CERRADA:
FASE 6 — INTEGRACIÓN DE MODELO LLM REAL (LOCAL)

ALCANCE DE LA FASE:
La Fase 6 queda oficialmente CERRADA tras haberse cumplido de forma
completa y verificable los siguientes puntos:

DISEÑO Y CONTROL:
- Rol del LLM claramente definido
- Arquitectura heredada de Fase 5 respetada
- Core mantiene autoridad absoluta
- LLM integrado como subsistema externo
- Flujo core → LLM → core definido y validado
- Activación del LLM explícita y controlada

SEGURIDAD Y ESTABILIDAD:
- Fallback definido y obligatorio
- Fallos del LLM no degradan el sistema
- LLM sin acceso a sistema, red o archivos
- Sin autonomía
- Sin memoria propia persistente
- Sin ejecución de código

RECURSOS Y RENDIMIENTO:
- Carga bajo demanda
- Descarga explícita
- Límites de tiempo definidos
- Límites de recursos definidos
- Capacidad de desactivar el LLM en cualquier momento

IMPLEMENTACIÓN BASE:
- Adaptador LLM real implementado
- Carga controlada del modelo
- Inferencia controlada y no persistente
- Fallback funcional garantizado
- Sistema plenamente operativo sin LLM

ESTADO DEL SISTEMA TRAS EL CIERRE:
- LLM REAL: IMPLEMENTADO A NIVEL DE INFRAESTRUCTURA
- LLM REAL: NO PROBADO AÚN (correcto)
- Core: INTACTO
- Arquitectura: ESTABLE
- Reversibilidad: TOTAL
- Deuda técnica: NULA

PROHIBICIONES A PARTIR DE ESTE CIERRE:
- No se modifica el diseño del LLM dentro de esta fase
- No se amplían capacidades del LLM aquí
- No se prueba el LLM fuera de una fase dedicada
- No se introduce IA adicional sin nueva fase

CONDICIÓN PARA AVANZAR:
La validación funcional del LLM REAL deberá realizarse
en una NUEVA FASE explícita e independiente.

FASE 6 CERRADA.

================================================================
ANEXO — APERTURA DE FASE 7: PRIMERA PRUEBA REAL CONTROLADA DEL LLM
================================================================

FECHA DE APERTURA: 2025-12-15

FASE ABIERTA:
FASE 7 — PRIMERA PRUEBA REAL CONTROLADA DEL LLM LOCAL

OBJETIVO DE LA FASE:
Validar por primera vez el funcionamiento de un MODELO LLM REAL
integrado en AURA, de forma controlada, mínima y reversible,
sin ampliar capacidades ni introducir cambios estructurales.

ALCANCE DE LA PRUEBA:
Esta fase se limita estrictamente a:

- Cargar un LLM REAL local mediante el adaptador existente
- Ejecutar UNA o pocas inferencias controladas
- Verificar que el flujo completo funciona:
  STT → core → adaptador LLM → core → TTS
- Confirmar que el sistema:
  - no se bloquea
  - no se degrada
  - mantiene control del core
  - retorna a estado estable

CRITERIOS DE LA PRUEBA:
- Entrada simple y controlada
- Prompt mínimo
- Sin contexto extendido
- Sin memoria conversacional
- Sin streaming
- Sin acciones
- Sin autonomía

CRITERIOS DE ÉXITO:
La fase se considera EXITOSA si:
- El modelo carga correctamente
- Se obtiene una respuesta textual válida
- El core decide la respuesta
- El TTS emite la respuesta
- El sistema vuelve a estado “Escuchando”
- El fallo del modelo (si ocurre) activa fallback sin romper AURA

CRITERIOS DE FALLO:
La fase se considera FALLIDA si:
- El sistema se bloquea
- El core pierde control
- El LLM introduce efectos colaterales
- No es posible recuperar estado estable

REGLAS DURANTE LA FASE:
- No se modifica el core
- No se amplía el adaptador
- No se ajustan prompts dinámicamente
- No se añade memoria
- No se introducen optimizaciones

CONDICIÓN DE CIERRE:
La fase se cerrará explícitamente como:
- EXITOSA, o
- FALLIDA (con rollback)

FASE 7 ABIERTA.

================================================================
ANEXO — CIERRE DE FASE 7: PRIMERA PRUEBA REAL CONTROLADA DEL LLM
================================================================

FECHA DE CIERRE: 2025-12-15

FASE CERRADA:
FASE 7 — PRIMERA PRUEBA REAL CONTROLADA DEL LLM LOCAL

RESULTADO DE LA FASE:
FASE EXITOSA

ALCANCE DE LA PRUEBA REAL:
Durante esta fase se ejecutaron pruebas reales y controladas del flujo
completo de AURA con integración de LLM REAL, validando el sistema
en condiciones operativas mínimas y seguras.

PRUEBAS REALIZADAS:
- Entrada por interfaz textual (UI)
- Procesamiento por el core
- Evaluación de reglas deterministas (Fase 4)
- Escalado controlado al adaptador LLM real
- Activación de fallback ante ausencia de respuesta válida
- Retorno del sistema a estado estable

RESULTADOS OBSERVADOS:
- El sistema responde correctamente a entradas simples
- El core mantiene autoridad absoluta
- El flujo UI → core → LLM → core → TTS funciona sin bloqueo
- El fallback del LLM se activa de forma correcta y controlada
- La aplicación no se bloquea ni se degrada
- El estado del sistema permanece coherente
- La UI continúa operativa tras la prueba

CRITERIOS DE ÉXITO VERIFICADOS:
- Integración del LLM real no rompe AURA
- Fallos del LLM no afectan estabilidad
- El core decide cuándo escalar
- El sistema vuelve a estado “Escuchando”
- No existen efectos colaterales

ESTADO DEL LLM TRAS LA FASE:
- LLM REAL: INTEGRADO A NIVEL DE INFRAESTRUCTURA
- LLM REAL: FUNCIONAMIENTO VALIDADO EN MODO CONTROLADO
- Inteligencia del modelo: NO EVALUADA (fuera de alcance)
- Dependencia del LLM: NULA

PROHIBICIONES A PARTIR DE ESTE CIERRE:
- No se amplían pruebas dentro de esta fase
- No se evalúa calidad cognitiva aquí
- No se ajusta comportamiento del modelo
- No se introducen nuevas capacidades

CONDICIÓN PARA AVANZAR:
La siguiente fase corresponde exclusivamente a la
CONSOLIDACIÓN, SELLADO Y DECLARACIÓN DE AURA v1.

FASE 7 CERRADA.

================================================================
ANEXO — APERTURA DE FASE 8: CONSOLIDACIÓN Y SELLADO DE AURA v1
================================================================

FECHA DE APERTURA: 2025-12-16

FASE ABIERTA:
FASE 8 — CONSOLIDACIÓN Y SELLADO DE AURA v1

OBJETIVO DE LA FASE:
Cerrar formalmente AURA v1 como sistema funcional, estable y controlado,
eliminando ambigüedades, sellando componentes base y declarando
la versión como lista a nivel de arquitectura e implementación.

ALCANCE DE LA FASE:
Esta fase NO introduce nuevas capacidades.
Esta fase NO amplía IA.
Esta fase NO modifica el flujo funcional validado.

Incluye exclusivamente:
- Consolidación de arquitectura final
- Sellado del core como estable
- Identificación y fijación de interfaces públicas
- Revisión y aceptación de componentes puente
- Declaración formal de AURA v1

ELEMENTOS A CONSOLIDAR:
- Core (orquestación, estados, decisiones)
- Adaptador LLM (real, controlado)
- Capa de voz (STT/TTS) como periférica
- UI como interfaz técnica válida
- Flujo completo validado end-to-end

PROHIBICIONES DURANTE LA FASE:
- No se agregan features
- No se cambian decisiones de diseño
- No se optimiza prematuramente
- No se reabre ninguna fase cerrada
- No se introduce wake word
- No se cambia STT/TTS

CRITERIOS DE ÉXITO:
La Fase 8 se considerará completada cuando:
- El core quede sellado como estable
- Las interfaces queden claramente definidas
- El sistema sea reproducible
- No existan pasos pendientes
- Se declare formalmente AURA v1

CONDICIÓN DE CIERRE:
La fase se cerrará explícitamente con un
ANEXO DE CIERRE Y DECLARACIÓN DE AURA v1.

FASE 8 ABIERTA.

================================================================
ANEXO — FASE 8.1: CONSOLIDACIÓN DEL CORE (SELLADO)
================================================================

FECHA: 2025-12-16

OBJETIVO:
Sellar el CORE de AURA v1 como componente estable,
definiendo de forma explícita sus responsabilidades,
interfaces públicas y prohibiciones definitivas.

PRINCIPIO FUNDAMENTAL:
El core es el ORQUESTADOR del sistema.
No escucha, no habla, no ejecuta acciones físicas,
no depende de hardware ni de interfaces concretas.

RESPONSABILIDADES DEFINITIVAS DEL CORE:
- Recibir texto de entrada (desde STT o UI)
- Mantener y publicar estado interno
- Decidir flujo de respuesta (reglas vs LLM)
- Orquestar llamadas a subsistemas
- Emitir texto de salida hacia TTS

INTERFACES PÚBLICAS DEL CORE (FIJADAS):
- process_text(text: str) -> str
- get_status() -> str
- register_listener(callback)

Estas interfaces quedan CONGELADAS para AURA v1.

INTERFACES NO PÚBLICAS (INTERNAS):
- Manejo de estados
- Lógica de escalado a LLM
- Gestión de fallback
- Orquestación interna

PROHIBICIONES DEFINITIVAS EN EL CORE:
- No acceso directo a micrófono
- No acceso directo a audio
- No implementación de wake word
- No ejecución de código externo
- No memoria conversacional persistente
- No autonomía

DEPENDENCIAS PERMITIDAS:
- Adaptador LLM (vía interfaz definida)
- Subsistema de reglas deterministas
- Subsistema de estado
- Subsistema TTS (solo como salida de texto)

DEPENDENCIAS PROHIBIDAS:
- STT directo
- UI específica
- Motores de voz concretos
- Modelos IA embebidos

ESTADO TRAS ESTE ANEXO:
- Core considerado ESTABLE
- Core considerado SELLADO para AURA v1
- Cambios futuros al core implican nueva versión (v2)

FASE 8.1 DEFINIDA.

================================================================
ANEXO — FASE 8.2: CONSOLIDACIÓN DEL ADAPTADOR LLM (SELLADO)
================================================================

FECHA: 2025-12-16

OBJETIVO:
Sellar el ADAPTADOR LLM como componente estable y reemplazable,
definiendo de forma definitiva su contrato, límites y responsabilidades
dentro de AURA v1.

PRINCIPIO FUNDAMENTAL:
El adaptador LLM es un PUENTE CONTROLADO.
Nunca es un agente.
Nunca es una autoridad.
Nunca decide el flujo.

RESPONSABILIDADES DEFINITIVAS DEL ADAPTADOR LLM:
- Cargar un modelo LLM local bajo demanda
- Ejecutar inferencias de texto bajo solicitud explícita del core
- Retornar texto plano al core
- Gestionar errores internos del modelo
- Proveer fallback seguro cuando corresponda

INTERFAZ PÚBLICA DEL ADAPTADOR (FIJADA):
- request_response(input_text: str, context: dict | None) -> str
- load() -> bool
- unload()

Esta interfaz queda CONGELADA para AURA v1.

RESPONSABILIDADES EXPLÍCITAMENTE EXCLUIDAS:
- Decidir cuándo invocarse
- Mantener memoria conversacional
- Acceder a sistema, red o archivos
- Ejecutar acciones
- Controlar TTS o STT
- Emitir audio o texto directamente al usuario

POLÍTICA DE CONTROL:
- El adaptador solo responde a llamadas del core
- El core decide si la respuesta se usa o se descarta
- El adaptador no conoce el estado global del sistema

POLÍTICA DE FALLOS:
- Cualquier fallo interno es contenido
- Nunca se propagan excepciones al core
- Siempre se retorna una respuesta segura o fallback
- El fallo del modelo no degrada AURA

POLÍTICA DE REEMPLAZO:
- El adaptador puede cambiar de backend (llama, phi, otro)
- El core NO se modifica
- La arquitectura NO se altera

DEPENDENCIAS PERMITIDAS:
- Librerías locales de inferencia
- Modelos locales configurados externamente

DEPENDENCIAS PROHIBIDAS:
- Servicios cloud
- APIs externas
- Dependencias no controladas

ESTADO TRAS ESTE ANEXO:
- Adaptador LLM considerado ESTABLE
- Contrato de integración SELLADO
- Cambios futuros implican nueva versión (v2)

FASE 8.2 DEFINIDA.

================================================================
ANEXO — FASE 8.3: CONSOLIDACIÓN DE LA CAPA DE VOZ (STT / TTS)
================================================================

FECHA: 2025-12-16

OBJETIVO:
Sellar la CAPA DE VOZ de AURA v1 como subsistema periférico,
intercambiable y desacoplado del core, definiendo de forma definitiva
sus responsabilidades, límites y relación con el sistema central.

PRINCIPIO FUNDAMENTAL:
La voz NO es inteligencia.
La voz NO decide.
La voz NO controla el sistema.
La voz es una interfaz de entrada y salida.

COMPONENTES DE LA CAPA DE VOZ:
- STT (Speech To Text)
- TTS (Text To Speech)

Ambos componentes residen FUERA del core.

RESPONSABILIDADES DEFINITIVAS DE STT:
- Capturar audio desde el micrófono
- Convertir voz en texto
- Entregar texto al core por interfaz definida
- No interpretar intención
- No filtrar contenido semántico
- No decidir activación lógica

RESPONSABILIDADES DEFINITIVAS DE TTS:
- Recibir texto desde el core
- Convertir texto en audio
- Emitir voz al usuario
- No modificar contenido
- No decidir cuándo hablar
- No mantener estado conversacional

INTERFAZ CON EL CORE:
- STT → core: texto plano
- core → TTS: texto plano

No existen otras dependencias directas.

PROHIBICIONES DEFINITIVAS EN LA CAPA DE VOZ:
- No lógica de negocio
- No acceso al LLM
- No acceso al estado interno del core
- No decisiones autónomas
- No memoria persistente

WAKE WORD (PALABRA DE ACTIVACIÓN):
- No forma parte de AURA v1
- Si se implementa en el futuro:
  - Vivirá en la capa de voz
  - Antes del STT normal
  - Fuera del core y del LLM

POLÍTICA DE INTERCAMBIO:
- STT puede ser reemplazado sin tocar el core
- TTS puede ser reemplazado sin tocar el core
- Voces, motores o proveedores son intercambiables

ESTADO TRAS ESTE ANEXO:
- Capa de voz considerada ESTABLE
- STT/TTS sellados como periféricos
- Core completamente desacoplado de voz

FASE 8.3 DEFINIDA.

================================================================
ANEXO — FASE 8.4: CONSOLIDACIÓN DE LA INTERFAZ (UI TÉCNICA)
================================================================

FECHA: 2025-12-16

OBJETIVO:
Consolidar la INTERFAZ DE USUARIO (UI) de AURA v1 como una
interfaz técnica válida, suficiente y estable, sin pretensión
de producto final, definiendo su alcance y límites definitivos.

PRINCIPIO FUNDAMENTAL:
La UI NO es el sistema.
La UI NO contiene lógica.
La UI NO decide comportamiento.
La UI es un MEDIO de interacción.

ROL DEFINITIVO DE LA UI EN AURA v1:
- Proveer entrada de texto al core
- Mostrar respuestas del sistema
- Mostrar estado actual de AURA
- Permitir pruebas y uso técnico controlado

RESPONSABILIDADES DEFINITIVAS DE LA UI:
- Capturar texto del usuario
- Enviar texto al core mediante interfaz pública
- Mostrar texto de salida devuelto por el core
- Reflejar estados (Escuchando, Procesando, Respondiendo)

RESPONSABILIDADES EXCLUIDAS DE LA UI:
- No contiene lógica de decisión
- No interactúa directamente con LLM
- No accede a STT o TTS
- No gestiona memoria
- No ejecuta acciones
- No interpreta intención

INTERFAZ CON EL CORE:
- UI → core.process_text(text)
- core → UI: texto de respuesta + estado

Esta interfaz queda FIJADA para AURA v1.

ALCANCE DE LA UI EN AURA v1:
- Interfaz técnica
- Funcional
- Estable
- Suficiente para uso real
- No optimizada para UX final

LIMITACIONES ACEPTADAS:
- Diseño simple
- Sin personalización avanzada
- Sin identidad visual final
- Sin animaciones complejas

Estas limitaciones son DELIBERADAS.

PROHIBICIONES DEFINITIVAS EN LA UI:
- No duplicar lógica del core
- No incluir reglas conversacionales
- No gestionar activación por voz
- No persistir estado propio

ESTADO TRAS ESTE ANEXO:
- UI técnica considerada ESTABLE
- Flujo UI ↔ core consolidado
- UI final de producto queda fuera de AURA v1

FASE 8.4 DEFINIDA.

================================================================
ANEXO — FASE 8.5: CONSOLIDACIÓN DEL FLUJO COMPLETO DE AURA v1
================================================================

FECHA: 2025-12-16

OBJETIVO:
Declarar y sellar el FLUJO COMPLETO DE FUNCIONAMIENTO de AURA v1
de extremo a extremo, estableciendo el comportamiento definitivo
del sistema en condiciones normales y de fallo.

PRINCIPIO FUNDAMENTAL:
El flujo es LINEAL, CONTROLADO y ORQUESTADO por el core.
No existen flujos alternos ocultos ni comportamientos implícitos.

FLUJO NORMAL DE OPERACIÓN (END-TO-END):

1. Entrada del usuario
   - Vía UI (texto) o STT (voz)
   - La entrada siempre es TEXTO PLANO

2. Recepción por el core
   - core.process_text(text)
   - El core cambia estado a “Procesando”

3. Evaluación determinista
   - El core intenta resolver mediante reglas internas
   - Si existe respuesta válida → se utiliza

4. Escalado a LLM (si corresponde)
   - Solo si las reglas no resuelven
   - Invocación explícita al adaptador LLM
   - Inferencia controlada y con límites

5. Gestión de fallos
   - Si el LLM falla o no responde:
     - Se activa fallback seguro
     - El sistema continúa operando

6. Emisión de respuesta
   - El core devuelve TEXTO PLANO
   - El estado cambia a “Respondiendo”
   - El texto se envía a TTS (si aplica)

7. Retorno a estado estable
   - Estado final: “Escuchando”
   - El sistema queda listo para nueva entrada

FLUJO EN CASO DE FALLO:
- Ningún fallo rompe el ciclo
- Ningún fallo bloquea el sistema
- El usuario recibe siempre una respuesta válida
- El sistema vuelve a estado estable

COMPORTAMIENTO GARANTIZADO:
- AURA nunca se queda bloqueada
- AURA nunca decide por sí misma
- AURA nunca ejecuta acciones no autorizadas
- AURA siempre mantiene control centralizado

PROHIBICIONES DEFINITIVAS:
- No bucles autónomos
- No auto-invocación del LLM
- No dependencia obligatoria de voz
- No dependencia obligatoria del LLM

ESTADO TRAS ESTE ANEXO:
- Flujo completo declarado
- Comportamiento final de AURA v1 sellado
- No existen comportamientos implícitos

FASE 8.5 DEFINIDA.

================================================================
ANEXO — CIERRE DE FASE 8 Y DECLARACIÓN OFICIAL DE AURA v1
================================================================

FECHA DE CIERRE: 2025-12-16

FASE CERRADA:
FASE 8 — CONSOLIDACIÓN Y SELLADO DE AURA v1

DECLARACIÓN OFICIAL:
Con el cierre de esta fase, AURA v1 queda declarada como
SISTEMA FUNCIONAL, ESTABLE Y SELLADO.

ALCANCE DE AURA v1:
AURA v1 es una IA local que:
- Recibe texto por UI o voz
- Procesa entradas de forma controlada
- Responde mediante reglas deterministas o LLM local
- Mantiene control centralizado en el core
- Opera con fallback seguro
- Retorna siempre a un estado estable

COMPONENTES SELLADOS:
- Core: SELLADO como orquestador estable
- Adaptador LLM: SELLADO como subsistema controlado
- Capa de voz (STT/TTS): SELLADA como periférica
- UI técnica: SELLADA como interfaz válida
- Flujo end-to-end: SELLADO y documentado

GARANTÍAS FINALES:
- No autonomía
- No ejecución de acciones no autorizadas
- No dependencia obligatoria de LLM
- No dependencia obligatoria de voz
- No bucles autónomos
- No deuda técnica conocida

PROHIBICIONES POSTERIORES:
- No modificar el core dentro de AURA v1
- No ampliar capacidades dentro de AURA v1
- No introducir nuevas decisiones de diseño
- No reabrir fases cerradas

CRITERIO DE VERSIONADO:
Cualquier cambio funcional, arquitectónico o de alcance
posterior a este anexo pertenece a una NUEVA VERSIÓN
(AURA v2 o superior).

ESTADO FINAL:
- AURA v1: TERMINADA
- AURA v1: OPERATIVA
- AURA v1: SELLADA

FIN DE AURA v1.
================================================================
ANEXO — CIERRE FORMAL DE FASE 8: CONSOLIDACIÓN Y SELLADO DE AURA v1
================================================================

FECHA DE CIERRE: 2025-12-16

FASE CERRADA:
FASE 8 — CONSOLIDACIÓN Y SELLADO DE AURA v1

DECLARACIÓN:
Con este anexo se REAFIRMA y SE CIERRA FORMALMENTE la Fase 8,
dejando AURA v1 declarada como versión terminada, estable y sellada.

ALCANCE CONFIRMADO:
Durante la Fase 8 se consolidaron y sellaron definitivamente:

- Core como orquestador estable
- Interfaces públicas del core
- Adaptador LLM como subsistema controlado
- Capa de voz (STT/TTS) como periférica
- UI técnica como interfaz válida
- Flujo completo end-to-end
- Comportamiento normal y de fallo

ESTADO FINAL DE AURA v1:
- Funcional
- Estable
- Controlada
- Reproducible
- Sin deuda técnica conocida

GARANTÍAS REAFIRMADAS:
- El core no tiene autonomía
- El LLM no decide ni actúa
- La voz no controla lógica
- El sistema nunca queda bloqueado
- El fallback es obligatorio
- El control es siempre externo

PROHIBICIONES POST-CIERRE:
- No se modifica ningún componente de AURA v1
- No se amplían capacidades dentro de v1
- No se reabren fases cerradas
- Cualquier cambio pertenece a AURA v2 o superior

CRITERIO DE CONTINUIDAD:
AURA v1 queda definitivamente CERRADA.
Cualquier trabajo futuro debe iniciar
mediante apertura explícita de una nueva versión.

FASE 8 CERRADA.
AURA v1 FINALIZADA.

================================================================
ANEXO — APERTURA DE AURA v2 / FASE 9: INTERFAZ DE PRODUCTO
================================================================

FECHA DE APERTURA: 2025-12-16

VERSIÓN ABIERTA:
AURA v2

FASE ABIERTA:
FASE 9 — INTERFAZ DE PRODUCTO (UI / UX)

CONTEXTO:
AURA v1 ha sido cerrada y sellada como sistema funcional, estable
y controlado. La Fase 9 inaugura AURA v2 y se enfoca exclusivamente
en la EXPERIENCIA DE USUARIO, sin modificar la arquitectura ni la IA.

OBJETIVO DE LA FASE:
Diseñar y construir la INTERFAZ DE PRODUCTO de AURA, elevando la
interfaz técnica de v1 a una experiencia usable, coherente y
presentable para usuarios finales.

PRINCIPIO FUNDAMENTAL:
La interfaz NO define inteligencia.
La interfaz NO define decisiones.
La interfaz NO contiene lógica de negocio.
La interfaz consume interfaces ya selladas.

ALCANCE DE LA FASE:
Incluye:
- Diseño de UX (flujos, estados, feedback)
- Diseño visual (identidad, layout, estilo)
- Integración visual de estados del core
- Integración de entrada/salida de texto
- Preparación para identidad de voz (Nova)
- Animaciones y microinteracciones (si aplica)

EXCLUYE EXPLÍCITAMENTE:
- Cambios al core
- Cambios al adaptador LLM
- Cambios a STT/TTS
- Wake word
- Automatización
- Empaquetado
- Instalador

INTERFACES CONSUMIDAS (FIJADAS):
- core.process_text(text)
- core.get_status()
- eventos de estado (listeners)

CRITERIOS DE ÉXITO:
La Fase 9 se considera exitosa cuando:
- La UI es usable por un usuario no técnico
- El estado del sistema es claro y visible
- La experiencia es coherente y estable
- No se introduce deuda técnica
- El core y la IA permanecen intactos

REGLAS DE LA FASE:
- No se modifica ningún contrato sellado en v1
- La UI es reemplazable
- Las decisiones son de UX, no de arquitectura
- Cualquier experimento visual es aislado

ESTADO:
FASE ABIERTA.
IMPLEMENTACIÓN PENDIENTE.

AURA v2 — FASE 9 ABIERTA.

================================================================
ANEXO — AURA v2 / FASE 9.1: ALCANCE DE LA INTERFAZ DE PRODUCTO
================================================================

FECHA: 2025-12-16

OBJETIVO:
Definir de forma explícita el ALCANCE DE LA INTERFAZ DE PRODUCTO
de AURA, determinando qué información y controles son visibles
para el usuario final y cuáles permanecen internos al sistema.

PRINCIPIO FUNDAMENTAL:
El usuario no debe ver la complejidad del sistema.
El sistema no debe ocultar su estado operativo básico.

QUÉ VE EL USUARIO (VISIBLE):

- Campo de entrada de texto
- Área de respuesta de AURA
- Indicador de estado del sistema:
  - Escuchando
  - Procesando
  - Respondiendo
- Confirmación visual de actividad
- Mensajes de error amigables y no técnicos
- Identidad visual de AURA (nombre, estilo)

QUÉ NO VE EL USUARIO (OCULTO):

- Lógica interna del core
- Decisiones de escalado a LLM
- Errores internos del modelo
- Detalles técnicos de STT / TTS
- Logs del sistema
- Excepciones técnicas
- Configuraciones internas
- Estados intermedios no relevantes

CONTROLES DISPONIBLES AL USUARIO:

- Enviar texto
- Cancelar entrada actual (si aplica)
- Limpiar conversación visible

CONTROLES NO DISPONIBLES:

- Activar/desactivar LLM
- Cambiar backend de IA
- Manipular estados internos
- Forzar respuestas
- Acceder a memoria interna

FEEDBACK AL USUARIO:

- El sistema siempre responde algo
- El usuario nunca queda sin feedback
- El silencio prolongado está prohibido
- El estado visual sustituye mensajes técnicos

ROL DE LA INTERFAZ:
- Facilitar interacción
- Generar confianza
- Reducir fricción
- No enseñar arquitectura

CRITERIO DE ÉXITO DE ESTA SUBFASE:

- El usuario entiende qué está pasando
- El usuario no ve complejidad innecesaria
- La interfaz es clara y predecible
- No se filtra información técnica

ESTADO:
Alcance de interfaz definido.
Implementación pendiente.

FASE 9.1 DEFINIDA.

================================================================
ANEXO — AURA v2 / FASE 9.2: ESTADOS VISUALES Y FEEDBACK DE USUARIO
================================================================

FECHA: 2025-12-16

OBJETIVO:
Definir los ESTADOS VISUALES de AURA y el FEEDBACK asociado a cada uno,
garantizando que el usuario comprenda en todo momento qué está haciendo
el sistema sin necesidad de información técnica.

PRINCIPIO FUNDAMENTAL:
El usuario no debe adivinar.
El sistema debe comunicar estado, no implementación.

ESTADOS VISUALES DEFINITIVOS:

1. ESTADO: ESCUCHANDO
   - Indicador visual: reposo / animación suave
   - Mensaje opcional: “Estoy escuchando”
   - Input habilitado
   - No hay animaciones intrusivas

2. ESTADO: PROCESANDO
   - Indicador visual: animación de carga discreta
   - Mensaje: “Procesando…”
   - Input deshabilitado temporalmente
   - El usuario entiende que la solicitud fue recibida

3. ESTADO: RESPONDIENDO
   - Indicador visual: transición activa
   - Aparición progresiva del texto
   - Si hay TTS, sincronía visual con voz

4. ESTADO: ERROR CONTROLADO
   - Mensaje amigable y humano
   - Nunca técnico
   - Ejemplo: “Ahora mismo no puedo responder a eso”
   - El sistema vuelve automáticamente a “Escuchando”

TRANSICIONES PERMITIDAS:
- Escuchando → Procesando
- Procesando → Respondiendo
- Respondiendo → Escuchando
- Cualquier estado → Error controlado → Escuchando

TRANSICIONES PROHIBIDAS:
- Saltos sin feedback
- Estados silenciosos prolongados
- Estados ambiguos
- Estados técnicos expuestos

POLÍTICA DE FEEDBACK:

- Todo input del usuario recibe feedback
- El feedback es inmediato (visual)
- La latencia nunca es silenciosa
- El usuario no queda en duda

SINCRONIZACIÓN CON EL CORE:
- Los estados visuales reflejan estados reales del core
- No se inventan estados en la UI
- La UI escucha eventos, no los genera

PROHIBICIONES DEFINITIVAS:
- No mostrar logs
- No mostrar stack traces
- No mostrar decisiones internas
- No mostrar nombres de componentes

CRITERIO DE ÉXITO DE ESTA SUBFASE:
- El usuario siempre sabe qué está pasando
- El sistema se percibe vivo y confiable
- No hay confusión durante la interacción

ESTADO:
Estados visuales definidos.
Feedback consolidado.
Implementación pendiente.

FASE 9.2 DEFINIDA.

================================================================
ANEXO — AURA v2 / FASE 9.3: IDENTIDAD VISUAL Y PERSONALIDAD (NOVA)
================================================================

FECHA: 2025-12-16

OBJETIVO:
Definir la IDENTIDAD VISUAL y la PERSONALIDAD percibida de AURA
(en adelante “Nova”) como capa de experiencia, sin alterar
la inteligencia, la lógica ni el comportamiento del sistema.

PRINCIPIO FUNDAMENTAL:
La personalidad es PRESENTACIÓN.
La inteligencia es FUNCIÓN.
Ambas están estrictamente separadas.

NOMBRE DE EXPERIENCIA:
- Nombre visible: Nova
- AURA permanece como nombre del sistema interno
- El usuario interactúa con “Nova”
- El sistema sigue siendo AURA

ROL DE NOVA:
- Representación visual y sonora de AURA
- Voz, tono y presencia
- No toma decisiones
- No controla lógica
- No tiene estado propio

IDENTIDAD VISUAL (LINEAMIENTOS):

- Estilo: limpio, moderno, calmado
- Presencia: discreta, no invasiva
- Movimiento: suave, reactivo al estado
- Colores: paleta reducida y coherente
- Tipografía: legible, sin protagonismo excesivo

No se busca hiperrealismo ni simulación humana.

IDENTIDAD SONORA (LINEAMIENTOS):

- Voz clara y estable
- Ritmo natural
- Tono neutral y confiable
- Sin dramatización
- Sin emociones simuladas excesivas

La voz comunica estado, no intención propia.

PERSONALIDAD PERCIBIDA:

- Clara
- Respetuosa
- Directa
- No invasiva
- Sin afirmaciones de conciencia
- Sin referencias a “pensar” o “sentir”

Ejemplos permitidos:
- “Puedo ayudarte con eso”
- “Ahora mismo no tengo esa información”

Ejemplos prohibidos:
- “Yo pienso que…”
- “Siento que…”
- “Quiero hacer…”

RELACIÓN CON EL USUARIO:

- Asistencia bajo demanda
- No proactividad autónoma
- No interrupciones no solicitadas
- No dependencia emocional inducida

CONFIGURABILIDAD:

- La identidad puede ajustarse visualmente
- La voz puede cambiarse
- El nombre visible puede cambiarse
- Nada de esto altera el core

CRITERIO DE ÉXITO DE ESTA SUBFASE:

- El usuario percibe coherencia
- No hay confusión entre sistema y personaje
- La experiencia es confiable
- La identidad no interfiere con la función

ESTADO:
Identidad visual y personalidad definidas.
Implementación pendiente.

FASE 9.3 DEFINIDA.

================================================================
ANEXO — AURA v2 / FASE 9.4: LAYOUT, COMPONENTES Y ESTRUCTURA DE LA UI
================================================================

FECHA: 2025-12-16

OBJETIVO:
Definir la ESTRUCTURA VISUAL y los COMPONENTES de la interfaz de
producto de AURA (Nova), estableciendo un layout claro, consistente
y extensible, sin introducir lógica de negocio.

PRINCIPIO FUNDAMENTAL:
La estructura guía la experiencia.
Los componentes presentan estado, no lo crean.

LAYOUT GENERAL (ALTO NIVEL):

- Contenedor principal (viewport)
- Área de identidad (Nova)
- Área de conversación
- Área de entrada
- Indicador de estado

El layout es RESPONSIVO y centrado en la interacción.

DESCRIPCIÓN DE ÁREAS:

1. ÁREA DE IDENTIDAD (HEADER / AVATAR)
   - Representación visual de Nova
   - Animación suave ligada al estado
   - No interactiva (decorativa / informativa)

2. ÁREA DE CONVERSACIÓN (BODY)
   - Historial visible de intercambio
   - Mensajes del usuario y de Nova diferenciados
   - Scroll controlado
   - Sin edición retroactiva de mensajes

3. ÁREA DE ENTRADA (FOOTER)
   - Campo de texto
   - Botón de envío
   - Envío por Enter (configurable)
   - Input deshabilitado durante “Procesando”

4. INDICADOR DE ESTADO (OVERLAY / INLINE)
   - Refleja estados del core:
     Escuchando / Procesando / Respondiendo
   - Nunca muestra estados técnicos

COMPONENTES DEFINIDOS:

- AvatarNova
- StatusIndicator
- MessageList
- MessageBubble (User / Nova)
- TextInput
- SendButton

Cada componente:
- Es visual
- Es reemplazable
- No contiene lógica de negocio
- Consume props/eventos externos

GESTIÓN DE ESTADO EN LA UI:

- Estado visual derivado del core
- Sin estado global complejo
- Sin duplicación de lógica
- La UI reacciona, no decide

EXTENSIBILIDAD CONTROLADA:

- Se permite añadir temas visuales
- Se permite cambiar layout secundario
- Se permite adaptar a móvil / escritorio
- No se permite alterar contratos del core

PROHIBICIONES DEFINITIVAS:

- No lógica de IA en componentes
- No acceso directo a LLM
- No timers autónomos
- No manejo de errores técnicos

CRITERIO DE ÉXITO DE ESTA SUBFASE:

- La interfaz es clara y ordenada
- El flujo visual acompaña al flujo real
- Los componentes son simples y reutilizables
- No se introduce deuda de UX

ESTADO:
Layout y componentes definidos.
Implementación pendiente.

FASE 9.4 DEFINIDA.
================================================================
ANEXO — AURA v2 / FASE 9.5: FLUJOS DE USUARIO Y CASOS DE USO BÁSICOS
================================================================

FECHA: 2025-12-16

OBJETIVO:
Definir los FLUJOS DE USUARIO principales y los CASOS DE USO BÁSICOS
de la interfaz de producto de AURA (Nova), garantizando una interacción
predecible, simple y coherente con el comportamiento sellado del sistema.

PRINCIPIO FUNDAMENTAL:
El usuario sigue un flujo natural.
El sistema guía sin imponer.

FLUJO PRINCIPAL — INTERACCIÓN BÁSICA:

1. Inicio de la aplicación
   - Nova visible en estado “Escuchando”
   - Campo de entrada habilitado
   - No mensajes intrusivos

2. Entrada del usuario
   - Usuario escribe texto
   - Pulsa enviar o Enter
   - Feedback visual inmediato

3. Procesamiento
   - Estado cambia a “Procesando”
   - Input deshabilitado temporalmente
   - Indicador visual activo

4. Respuesta del sistema
   - Estado cambia a “Respondiendo”
   - Mensaje de Nova aparece en la conversación
   - Si hay voz, se reproduce sincronizada

5. Retorno a espera
   - Estado vuelve a “Escuchando”
   - Input habilitado nuevamente
   - Sistema listo para nueva interacción

FLUJO ALTERNATIVO — ERROR CONTROLADO:

1. Usuario envía entrada
2. El sistema no puede responder
3. Nova muestra mensaje amigable
4. El sistema vuelve a “Escuchando”
5. El usuario puede continuar

FLUJO DE USO POR VOZ (SI APLICA):

1. Usuario habla (STT activo)
2. Texto llega al core
3. Flujo idéntico al textual
4. La UI refleja el estado real

No existen flujos paralelos ni ocultos.

CASOS DE USO BÁSICOS DEFINIDOS:

- Saludo inicial
- Pregunta simple
- Pregunta no resuelta (fallback)
- Interacción repetida
- Uso prolongado sin reinicio

CASOS DE USO EXCLUIDOS EN ESTA FASE:

- Configuración avanzada
- Personalización profunda
- Historial persistente
- Modo multitarea
- Automatizaciones

GESTIÓN DE ERRORES EN UX:

- Errores siempre comunicados
- Lenguaje humano
- Sin mensajes técnicos
- Sin bloqueos visibles

CRITERIO DE ÉXITO DE ESTA SUBFASE:

- El usuario entiende cómo usar Nova sin instrucciones
- El flujo es natural y consistente
- No existen estados confusos
- El sistema se percibe confiable

ESTADO:
Flujos de usuario definidos.
Casos de uso básicos consolidados.
Implementación pendiente.

FASE 9.5 DEFINIDA.

================================================================
ANEXO — AURA v2 / FASE 9.6: LÍMITES DE LA INTERFAZ Y NO-ALCANCE
================================================================

FECHA: 2025-12-16

OBJETIVO:
Definir de forma explícita los LÍMITES de la interfaz de producto
de AURA (Nova), estableciendo qué comportamientos, controles y
capacidades quedan FUERA del alcance de esta fase para evitar
deriva funcional y deuda de UX.

PRINCIPIO FUNDAMENTAL:
Lo que no se define explícitamente como permitido,
queda explícitamente prohibido.

NO-ALCANCE FUNCIONAL (PROHIBIDO EN LA UI):

- No configuración avanzada del sistema
- No toggles técnicos (LLM on/off, backend, modelos)
- No visualización de logs o diagnósticos
- No edición de prompts
- No control de memoria interna
- No ejecución manual de acciones
- No paneles de “admin”
- No scripting
- No plugins

NO-ALCANCE DE EXPERIENCIA:

- No personalidad dinámica
- No emociones simuladas
- No proactividad no solicitada
- No interrupciones automáticas
- No “sugerencias” espontáneas
- No multitarea visible

NO-ALCANCE VISUAL:

- No dashboards complejos
- No gráficas técnicas
- No indicadores de rendimiento
- No visualización de tokens
- No métricas de IA

NO-ALCANCE DE INTERACCIÓN:

- No comandos especiales ocultos
- No atajos técnicos documentados solo para expertos
- No modos secretos
- No flujos paralelos

JUSTIFICACIÓN DEL NO-ALCANCE:

- Mantener simplicidad
- Proteger contratos sellados en v1
- Evitar deuda de producto prematura
- Garantizar claridad para el usuario final
- Facilitar empaquetado posterior

CRITERIOS DE ACEPTACIÓN:

- Si una funcionalidad requiere explicar “cómo funciona internamente”,
  queda fuera.
- Si una funcionalidad requiere documentación técnica,
  queda fuera.
- Si una funcionalidad cambia decisiones del core,
  queda fuera.

EVOLUCIÓN FUTURA:

Todo lo excluido en este anexo:
- Puede evaluarse en fases futuras
- Requiere apertura explícita de nueva fase
- No se introduce por acumulación incremental

ESTADO:
Límites de interfaz definidos.
No-alcance declarado.
Implementación protegida.

FASE 9.6 DEFINIDA.

================================================================
ANEXO — AURA v2 / FASE 9.7: CHECKLIST DE ENTRADA A IMPLEMENTACIÓN UI
================================================================

FECHA: 2025-12-16

OBJETIVO:
Establecer la PUERTA FINAL DE CONTROL antes de iniciar la
IMPLEMENTACIÓN DE LA INTERFAZ DE PRODUCTO (UI) de AURA v2,
garantizando que el diseño esté completo, el alcance acotado
y la arquitectura protegida.

PRINCIPIO FUNDAMENTAL:
La interfaz se implementa cuando ya no se discute qué es,
qué hace y qué no hace.

CHECKLIST OBLIGATORIO (TODOS DEBEN CUMPLIRSE):

ALCANCE Y DISEÑO
- Paso 9.1 (alcance visible) definido
- Paso 9.2 (estados y feedback) definido
- Paso 9.3 (identidad Nova) definida
- Paso 9.4 (layout y componentes) definido
- Paso 9.5 (flujos de usuario) definido
- Paso 9.6 (límites y no-alcance) definido

ARQUITECTURA
- Core sellado (v1)
- Interfaces del core congeladas
- Adaptador LLM intacto
- Capa de voz desacoplada
- UI sin lógica de negocio

CONTROL
- La UI consume interfaces existentes
- La UI no toma decisiones
- La UI no maneja estados internos propios
- La UI es reemplazable

RIESGO
- No se modifica IA
- No se modifica core
- No se modifica flujo
- Riesgo limitado a capa visual

IMPLEMENTACIÓN
- Tecnología de UI decidida (framework / stack)
- Primer archivo a crear identificado
- Estructura de carpetas definida
- Implementación incremental prevista
- Cambios fácilmente reversibles

CRITERIO DE AUTORIZACIÓN:
La implementación de la UI puede comenzar SOLO si:
- Este checklist está completo
- El usuario autoriza explícitamente “Iniciar implementación UI”

ESTADO:
Checklist completo.
Implementación BLOQUEADA hasta orden explícita.

FASE 9.7 DEFINIDA.

================================================================
ANEXO — AURA v2 / FASE 9.12: PREPARACIÓN PARA ESTÉTICA Y TEMAS
================================================================

FECHA: 2025-12-16

OBJETIVO:
Definir los PUNTOS DE EXTENSIÓN VISUAL de la UI de AURA (Nova) para
permitir estética, temas y ajustes visuales futuros, sin alterar
comportamiento, lógica ni contratos existentes.

PRINCIPIO FUNDAMENTAL:
La estética se INYECTA.
El comportamiento NO se toca.

ALCANCE DE ESTE PASO:
- Definir QUÉ se podrá tematizar
- Definir DÓNDE se conectará la estética
- Definir QUÉ NO se cambia
- No implementar estilos ni temas aún

PUNTOS DE EXTENSIÓN VISUAL (DEFINIDOS):

1. TIPOGRAFÍA
   - Familias permitidas
   - Tamaños base
   - Jerarquía (título, estado, mensaje)
   - Sin cambios dinámicos por lógica

2. PALETA DE COLORES
   - Colores de fondo
   - Colores de texto
   - Colores de acento
   - Estados (escuchando / procesando / respondiendo)
   - Sin semántica funcional (solo visual)

3. COMPONENTES TEMATIZABLES
   - Header / identidad
   - Indicador de estado
   - Burbujas de mensaje
   - Área de entrada
   - Botones

4. ANIMACIONES (OPCIONALES, FUTURAS)
   - Transiciones suaves de estado
   - Aparición de mensajes
   - Animaciones del avatar
   - Nunca bloqueantes
   - Nunca lógicas

5. AVATAR / IDENTIDAD VISUAL
   - Imagen / forma / animación
   - Vinculada SOLO a estados visuales
   - No reacciona a contenido semántico

MECANISMO DE APLICACIÓN (CONCEPTUAL):

- Estilos definidos en un módulo separado (ej. ui/theme.py)
- La UI consume valores de tema
- Cambiar tema NO cambia flujo
- Cambiar tema NO requiere tocar core

PROHIBICIONES DEFINITIVAS:
- No lógica en temas
- No estilos condicionales por contenido
- No temas que oculten estados
- No dependencia de IA para estética

CRITERIO DE ÉXITO DE ESTE PASO:
- La UI queda preparada para recibir estética
- No se introduce deuda
- No se altera comportamiento existente
- La implementación futura es limpia y localizada

ESTADO:
Puntos de extensión visual definidos.
Estética NO implementada.
Comportamiento protegido.

FASE 9.12 DEFINIDA.

================================================================
ANEXO — CIERRE DE AURA v2 / FASE 9: INTERFAZ DE PRODUCTO
================================================================

FECHA DE CIERRE: 2025-12-16

VERSIÓN:
AURA v2

FASE CERRADA:
FASE 9 — INTERFAZ DE PRODUCTO (UI / UX)

DECLARACIÓN:
Con este anexo se declara CERRADA la Fase 9 de AURA v2, quedando
la INTERFAZ DE PRODUCTO definida, implementada en su base funcional
y preparada para evolución estética sin afectar el sistema.

ALCANCE CERRADO EN ESTA FASE:
Durante la Fase 9 se realizó de forma completa y ordenada:

- Definición del alcance visible al usuario
- Definición de estados visuales y feedback
- Definición de identidad y personalidad (Nova)
- Definición de layout y componentes
- Definición de flujos de usuario
- Declaración explícita de no-alcance
- Checklist de entrada a implementación
- Implementación de UI base funcional
- Mejoras de UX básicas
- Micro-interacciones
- Preparación para estética y temas

ESTADO DE LA INTERFAZ TRAS EL CIERRE:
- UI funcional y estable
- UX clara y predecible
- Integración limpia con el core
- Sin lógica de negocio
- Sin dependencia de IA
- Preparada para tematización futura

GARANTÍAS REAFIRMADAS:
- El core permanece intacto
- La IA no se ve alterada
- La interfaz es reemplazable
- No existe deuda técnica conocida
- El comportamiento del sistema no cambia

PROHIBICIONES POST-CIERRE:
- No ampliar UI dentro de esta fase
- No introducir lógica en la interfaz
- No alterar contratos sellados
- Cambios posteriores requieren nueva fase

CRITERIO DE CONTINUIDAD:
Cualquier trabajo futuro relacionado con:
- Estética final
- Temas
- Avatar avanzado
- Wake word
- Empaquetado
- Instalador

pertenece a NUEVAS FASES de AURA v2.

FASE 9 CERRADA.

================================================================
ANEXO — APERTURA DE AURA v2 / FASE 11: WAKE WORD Y MODO MANOS LIBRES
================================================================

FECHA DE APERTURA: 2025-12-16

VERSIÓN:
AURA v2

FASE ABIERTA:
FASE 11 — DETECCIÓN DE PALABRA DE ACTIVACIÓN (WAKE WORD)

CONTEXTO:
AURA v1 está cerrada y estable.
La Fase 9 (Interfaz) ha sido cerrada exitosamente.
Esta fase introduce interacción por voz continua mediante
PALABRA DE ACTIVACIÓN, sin alterar el core ni la IA.

OBJETIVO DE LA FASE:
Permitir que AURA/Nova escuche de forma pasiva y se active
únicamente al detectar una PALABRA DE ACTIVACIÓN definida
(ej. “Nova”), habilitando interacción manos libres segura
y controlada.

PRINCIPIO FUNDAMENTAL:
La activación es EXTERNA al core.
El core nunca decide cuándo escuchar.
La detección de wake word vive en la CAPA DE VOZ.

ALCANCE DE LA FASE:
Incluye:
- Definición de la palabra de activación
- Detección pasiva y continua de wake word
- Habilitación/deshabilitación controlada de STT
- Integración limpia con la capa de voz existente
- Feedback visual/sonoro de activación

EXCLUYE EXPLÍCITAMENTE:
- Cambios al core
- Cambios al adaptador LLM
- Automatización de acciones
- Memoria avanzada
- Empaquetado
- Instalador

ARQUITECTURA DE ACTIVACIÓN (ALTO NIVEL):

Micrófono
→ Detector de wake word (FASE 11)
→ STT activo temporalmente
→ Texto al core
→ Core decide y responde
→ Retorno a escucha pasiva

RESPONSABILIDADES DEL DETECTOR DE WAKE WORD:
- Escuchar audio de forma pasiva
- Detectar palabra definida con alta precisión
- No interpretar intención
- No generar texto
- No acceder al core directamente
- No mantener estado conversacional

POLÍTICA DE CONTROL:
- Wake word configurable
- Activación explícita y temporal
- Tiempo máximo de escucha activa
- Retorno automático a modo pasivo

CRITERIOS DE ÉXITO:
La fase se considera exitosa cuando:
- La palabra de activación despierta a AURA
- No hay activaciones falsas frecuentes
- El core recibe texto solo tras activación
- El sistema vuelve a modo pasivo correctamente
- No se degrada el rendimiento del sistema

ESTADO:
FASE ABIERTA.
DISEÑO DETALLADO PENDIENTE.
IMPLEMENTACIÓN BLOQUEADA HASTA DEFINICIÓN COMPLETA.

AURA v2 — FASE 11 ABIERTA.

================================================================
ANEXO — AURA v2 / FASE 11.1: PALABRA DE ACTIVACIÓN (WAKE WORD)
================================================================

FECHA: 2025-12-16

OBJETIVO:
Definir la PALABRA DE ACTIVACIÓN (wake word) de AURA/Nova y los
CRITERIOS DE DETECCIÓN que regirán su funcionamiento, garantizando
activación confiable, controlada y con bajo índice de falsos positivos.

PRINCIPIO FUNDAMENTAL:
La activación es un EVENTO TÉCNICO.
No implica intención, comprensión ni decisión por parte del sistema.

PALABRA DE ACTIVACIÓN DEFINIDA:
- Palabra principal: “Nova”
- Pronunciación esperada: /ˈno.va/
- Idioma base: español neutro
- Variantes aceptadas: pronunciación natural sin acentos marcados

CRITERIOS DE ELECCIÓN DE LA PALABRA:
- Breve (2 sílabas)
- Sonoramente distintiva
- Baja frecuencia en habla cotidiana
- Fácil pronunciación
- Identidad coherente con la experiencia

CRITERIOS DE DETECCIÓN (ALTO NIVEL):

- Detección basada en audio, no en texto
- Coincidencia fonética aproximada
- Tolerancia a ruido moderado
- Sensibilidad ajustable
- Umbral mínimo de confianza requerido

CRITERIOS DE RECHAZO:
- No se activa con palabras similares no intencionadas
- No se activa con fragmentos de conversación
- No se activa por audio reproducido por el sistema
- No se activa por TTS de Nova

ALCANCE DE LA ACTIVACIÓN:
- La detección SOLO habilita STT
- La detección NO envía texto al core
- La detección NO ejecuta acciones
- La detección NO cambia estados internos del core

FEEDBACK DE ACTIVACIÓN:
- Señal visual inmediata (estado “Escuchando activo”)
- Señal sonora breve (opcional, no intrusiva)
- Confirmación clara para el usuario

CONFIGURABILIDAD:
- La palabra puede cambiarse en el futuro
- El cambio no altera el core
- El cambio no altera la IA
- El cambio requiere nueva fase de producto

CRITERIO DE ÉXITO DE ESTA SUBFASE:
- La palabra activa el sistema de forma consistente
- Los falsos positivos son raros
- El usuario percibe control y previsibilidad
- El sistema no se activa solo

ESTADO:
Palabra de activación definida.
Criterios de detección establecidos.
Implementación pendiente.

FASE 11.1 DEFINIDA.

================================================================
ANEXO — AURA v2 / FASE 11.2: ARQUITECTURA DEL DETECTOR DE WAKE WORD
================================================================

FECHA: 2025-12-16

OBJETIVO:
Definir la ARQUITECTURA del detector de palabra de activación
(wake word) de AURA/Nova, garantizando integración limpia,
desacoplamiento total del core y control absoluto del flujo.

PRINCIPIO FUNDAMENTAL:
El detector de wake word es un FILTRO PREVIO.
No pertenece al core.
No pertenece al LLM.
No pertenece a la UI.

UBICACIÓN ARQUITECTÓNICA:

voice/
├─ wake_word/
│  ├─ detector.py
│  ├─ config.py
│  └─ engine/
│     └─ (implementación específica)
├─ stt.py
└─ tts.py

El detector vive en la CAPA DE VOZ, antes del STT.

FLUJO ARQUITECTÓNICO DEFINITIVO:

Micrófono
→ Detector de wake word (pasivo)
→ (si se detecta “Nova”)
→ STT se habilita temporalmente
→ Texto generado
→ core.process_text(text)
→ Core decide
→ Respuesta → TTS
→ Retorno a escucha pasiva

RESPONSABILIDADES DEL DETECTOR:

- Capturar audio de bajo nivel
- Analizar audio en tiempo real
- Detectar palabra de activación
- Emitir evento de activación
- Habilitar STT durante una ventana controlada

RESPONSABILIDADES EXCLUIDAS:

- No convierte voz a texto
- No interpreta intención
- No envía datos al core
- No accede al LLM
- No maneja estados del sistema
- No decide cuándo responder

INTERFAZ DEL DETECTOR (CONCEPTUAL):

- start_listening()
- stop_listening()
- on_detected(callback)

El detector solo EMITE eventos.
No consume lógica.

POLÍTICA DE CONTROL:

- El detector puede activarse/desactivarse
- El sistema puede operar sin wake word
- El fallo del detector no rompe AURA
- El detector no mantiene estado persistente

AISLAMIENTO Y SEGURIDAD:

- El detector no graba audio
- El detector no guarda muestras
- El detector no transmite datos
- El detector no escucha TTS

CRITERIO DE ÉXITO DE ESTA SUBFASE:

- Arquitectura clara y desacoplada
- Core completamente aislado
- Flujo controlado y reversible
- Detector reemplazable

ESTADO:
Arquitectura del detector definida.
Implementación pendiente.

FASE 11.2 DEFINIDA.

================================================================
ANEXO — AURA v2 / FASE 11.3: MOTOR DE DETECCIÓN DE WAKE WORD
================================================================

FECHA: 2025-12-16

OBJETIVO:
Definir los CRITERIOS FORMALES para la selección del motor de
detección de palabra de activación (wake word), asegurando
precisión, bajo consumo y total control local.

PRINCIPIO FUNDAMENTAL:
La detección debe ser:
- Local
- Continua
- Liviana
- Confiable
- Reemplazable

CRITERIOS OBLIGATORIOS DEL MOTOR:

1. EJECUCIÓN LOCAL
   - No servicios cloud
   - No llamadas externas
   - Operación 100% offline

2. BAJO CONSUMO
   - Uso mínimo de CPU
   - Uso mínimo de memoria
   - Adecuado para escucha continua

3. LATENCIA BAJA
   - Detección casi inmediata
   - No bloquea STT ni core

4. PRECISIÓN
   - Baja tasa de falsos positivos
   - Sensibilidad ajustable
   - Tolerante a ruido moderado

5. INTEGRACIÓN LIMPIA
   - API simple
   - Fácil encapsulación
   - Sin dependencias invasivas

MOTORES CANDIDATOS ACEPTABLES:

- **Porcupine (Picovoice)**
  - Alta precisión
  - Optimizado para wake words
  - Modelos entrenables
  - Licencia a revisar

- **Vosk (wake word básico)**
  - Totalmente open-source
  - Precisión moderada
  - Mayor consumo que Porcupine

- **Snowboy (descartado)**
  - Proyecto discontinuado
  - No se recomienda

DECISIÓN DE REFERENCIA (NO VINCULANTE AÚN):

- Motor preferido: **Porcupine**
- Alternativa open-source: **Vosk**

La elección final:
- No altera el core
- No altera la IA
- No altera la UI
- Solo afecta la capa de voz

CRITERIOS DE DESCARTE:

Un motor será descartado si:
- Requiere conexión externa
- Introduce latencia perceptible
- Consume recursos excesivos
- No permite control de sensibilidad
- No permite aislamiento del sistema

CRITERIO DE ÉXITO DE ESTA SUBFASE:

- Motor seleccionado conceptualmente
- Riesgos identificados
- Alternativa definida

ESTADO:
Criterios de selección definidos.
Motor preferido identificado.
Implementación pendiente.

FASE 11.3 DEFINIDA.

================================================================
ANEXO — AURA v2 / FASE 11.4: FLUJO DE ACTIVACIÓN Y VENTANA DE ESCUCHA
================================================================

FECHA: 2025-12-16

OBJETIVO:
Definir el FLUJO EXACTO de activación por wake word y la
VENTANA DE ESCUCHA del STT, garantizando control, previsibilidad
y retorno automático a escucha pasiva.

PRINCIPIO FUNDAMENTAL:
La activación es TEMPORAL.
El silencio cierra la escucha.
El sistema siempre vuelve a estado pasivo.

FLUJO DE ACTIVACIÓN DEFINITIVO:

1. Modo pasivo
   - Detector de wake word activo
   - STT deshabilitado
   - Core no recibe texto

2. Detección de wake word (“Nova”)
   - Evento de activación emitido
   - Feedback inmediato (visual/sonoro)
   - STT se habilita

3. Ventana de escucha activa
   - STT captura voz del usuario
   - Conversión voz → texto
   - Texto enviado al core
   - Core procesa normalmente

4. Cierre de ventana
   La ventana de escucha se cierra si ocurre cualquiera:
   - Se recibe una entrada válida de texto
   - Se supera el tiempo máximo de escucha
   - Se detecta silencio prolongado
   - El usuario cancela (si existe gesto/acción)

5. Retorno a modo pasivo
   - STT deshabilitado
   - Detector de wake word permanece activo
   - Sistema listo para nueva activación

VENTANA DE ESCUCHA (PARÁMETROS):

- Duración máxima: 5–10 segundos (configurable)
- Detección de silencio: 1.5–2 segundos
- Una sola entrada por activación
- No encadenamiento automático de escuchas

POLÍTICA DE SEGURIDAD:

- El sistema no escucha continuamente con STT activo
- El audio no se almacena
- El audio no se retransmite
- La activación no persiste

FEEDBACK AL USUARIO:

- Activación confirmada de forma clara
- Estado visual: “Escuchando”
- Señal sonora breve (opcional)
- Cierre de escucha visible (retorno a reposo)

PROHIBICIONES DEFINITIVAS:

- No escucha permanente de STT
- No activación silenciosa
- No múltiples activaciones encadenadas
- No activación por TTS

CRITERIO DE ÉXITO DE ESTA SUBFASE:

- El usuario entiende cuándo hablar
- El sistema no queda “abierto”
- El control es siempre explícito
- El sistema vuelve solo a modo pasivo

ESTADO:
Flujo de activación definido.
Ventana de escucha establecida.
Implementación pendiente.

FASE 11.4 DEFINIDA.

================================================================
ANEXO — AURA v2 / FASE 11.5: FEEDBACK VISUAL Y SONORO DE ACTIVACIÓN
================================================================

FECHA: 2025-12-16

OBJETIVO:
Definir el FEEDBACK VISUAL y SONORO que confirma al usuario la
detección correcta de la palabra de activación (“Nova”) y el
inicio de la ventana de escucha activa, sin generar ambigüedad
ni interferir con el flujo del sistema.

PRINCIPIO FUNDAMENTAL:
El usuario debe SABER cuándo hablar.
El sistema no debe sorprender ni interrumpir.

FEEDBACK VISUAL (OBLIGATORIO):

Al detectar la wake word:
- Cambio inmediato del estado visible a “Escuchando”
- Animación suave del indicador de estado
- Refuerzo visual en el área de identidad (Nova)
- No se muestran mensajes técnicos
- No se bloquea la UI

Durante la ventana de escucha:
- Estado visible “Escuchando”
- Indicador activo persistente
- Claridad de que el sistema está atento

Al cierre de la ventana:
- Retorno visual a estado pasivo
- Eliminación del indicador activo
- Preparación para nueva activación

FEEDBACK SONORO (OPCIONAL, RECOMENDADO):

Al detectar la wake word:
- Sonido breve, neutro y no intrusivo
- Duración < 300 ms
- Volumen moderado
- No confusable con voz humana

Al cierre de la ventana (opcional):
- Sonido aún más sutil
- Indica fin de escucha activa

POLÍTICA DE SONIDO:

- El feedback sonoro es independiente del TTS
- El feedback no usa la voz de Nova
- El feedback no contiene lenguaje
- El feedback puede desactivarse

PROHIBICIONES DEFINITIVAS:

- No sonidos largos
- No frases habladas (“sí”, “te escucho”, etc.)
- No feedback ambiguo
- No sonidos que interrumpan al usuario
- No feedback sonoro continuo

COHERENCIA CON LA UI:

- El feedback visual siempre acompaña al sonoro
- Nunca hay sonido sin cambio visual
- Nunca hay cambio visual sin evento real

CRITERIO DE ÉXITO DE ESTA SUBFASE:

- El usuario sabe cuándo fue activado el sistema
- El usuario sabe cuándo hablar
- No hay confusión entre estados
- El feedback no molesta ni distrae

ESTADO:
Feedback de activación definido.
Implementación pendiente.

FASE 11.5 DEFINIDA.

================================================================
ANEXO — AURA v2 / FASE 11.6: CHECKLIST DE ENTRADA A IMPLEMENTACIÓN
================================================================

FECHA: 2025-12-16

OBJETIVO:
Establecer la PUERTA FINAL DE CONTROL antes de iniciar la
IMPLEMENTACIÓN del sistema de wake word, asegurando que
la arquitectura, el flujo y el feedback estén completamente
definidos y que no exista riesgo para el core o la IA.

PRINCIPIO FUNDAMENTAL:
El wake word se implementa solo cuando ya no se discute
qué es, dónde vive y cómo se comporta.

CHECKLIST OBLIGATORIO (TODOS DEBEN CUMPLIRSE):

DEFINICIÓN FUNCIONAL
- Paso 11.1 (palabra de activación) definido
- Paso 11.4 (flujo y ventana de escucha) definido
- Paso 11.5 (feedback de activación) definido

ARQUITECTURA
- Paso 11.2 (arquitectura del detector) definido
- Ubicación clara en capa de voz
- Core completamente desacoplado
- STT controlado externamente

TECNOLOGÍA
- Paso 11.3 (motor candidato) definido
- Alternativa identificada
- Riesgos conocidos
- Implementación local garantizada

CONTROL Y SEGURIDAD
- STT no siempre activo
- Ventana de escucha temporal
- Retorno automático a modo pasivo
- Sin almacenamiento de audio
- Sin transmisión externa

UI / UX
- Estados visuales preparados
- Feedback sonoro definido
- Coherencia con UI existente
- No interrupciones inesperadas

RIESGO
- Fallo del detector no bloquea AURA
- Wake word desactivable
- Sistema usable sin wake word
- Reversibilidad garantizada

CRITERIO DE AUTORIZACIÓN:
La implementación del wake word puede comenzar SOLO si:
- Este checklist está completo
- El usuario autoriza explícitamente
  “Iniciar implementación wake word”

ESTADO:
Checklist completo.
Implementación BLOQUEADA hasta orden explícita.

FASE 11.6 DEFINIDA.


================================================================
AUTORIDAD FINAL
================================================================
El usuario manda.
El asistente obedece.
Este archivo es la ÚNICA fuente de verdad.

FIN DEL BLOQUE MAESTRO
