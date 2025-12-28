# BLOQUE_MAESTRO_NOVA.md

## IDENTIDAD DEL PROYECTO

Nombre: NOVA  
Tipo: IA local con CLI conversacional  
Lenguaje principal: Python  
Modelo: LLaMA local (llama.cpp, GGUF)  
Modo: Offline (actual)  
Objetivo: Crear, editar y gestionar proyectos y archivos mediante lenguaje natural, con confirmaciones paso a paso, ejecución segura en sandbox y arquitectura extensible.

---

## ARQUITECTURA VÁLIDA (ÚNICA Y DEFINITIVA)

Flujo correcto y funcional:

CLI → Interpreter → Planner → Responder → Executor

Componentes eliminados y PROHIBIDOS en el estado actual:
- Router
- CognitiveRouter
- InternetLayer (desactivado)
- Reinyección de input
- Enrutamiento automático
- Ejecución sin confirmación

Si algo contradice esta arquitectura, este bloque maestro tiene prioridad absoluta.

---

## FLUJO CONVERSACIONAL OFICIAL

1. El usuario escribe una instrucción en lenguaje natural.
2. Interpreter:
   - Traduce a UN solo comando interno válido.
   - Comandos permitidos:
     - create_project <nombre>
     - create_file <archivo>
     - edit_file <archivo>
   - Devuelve una sola línea, sin texto adicional.
3. Planner:
   - Convierte el comando en una acción estructurada.
4. Responder:
   - Maneja TODO el estado conversacional.
   - Realiza confirmaciones paso a paso.
   - Mantiene estado `pending` hasta finalizar el flujo.
   - Es el único componente que se comunica con el usuario.
5. Executor:
   - Ejecuta en silencio.
   - No imprime mensajes de usuario.
   - Escribe únicamente dentro del sandbox.

---

## REGLAS DE UX (DECISIONES CERRADAS)

- Confirmaciones paso a paso: SÍ
- Ejecución automática sin permiso: NO
- Uso obligatorio de sandbox: SÍ
- Executor imprime mensajes: NO
- Responder es el único que habla con el usuario: SÍ
- El CLI NO debe reinterpretar input cuando existe `pending`: OBLIGATORIO
- LLaMA debe devolver una sola línea válida: OBLIGATORIO
- Cualquier acción sensible requiere confirmación humana: OBLIGATORIO

---

## SANDBOX Y RUTAS

Todas las operaciones de escritura se realizan exclusivamente en:

sandbox/software/

Ejemplo de proyecto válido:

sandbox/software/calculadora/
 ├─ main.py
 └─ README.md

---

## ESTADO PERSISTENTE DEL PROYECTO (ACTUAL)

Fases completadas:
- Fase 1: CLI base
- Fase 2: Comandos internos
- Fase 3: Validadores básicos
- Fase 4: Encadenamientos con confirmaciones

Funcionalidad confirmada y estable:
- Creación de proyectos con confirmación
- Propuesta de estructura
- Escritura de contenidos
- Correcciones de arquitectura resueltas
- Sin loops
- Sin repeticiones
- Sin logs de debug
- Sin reinyección de input
- Mensajes mostrados una sola vez

Última prueba válida:
- Proyecto "calculadora" creado correctamente en sandbox/software
- main.py y README.md generados
- Flujo completo sin errores

---

## CAPACIDADES FUTURAS DECLARADAS (NO ACTIVAS)

Las siguientes capacidades **NO están implementadas aún**, pero **están declaradas como objetivos formales** del proyecto y **solo se activarán cuando NOVA esté considerada “al 100%”** según criterios técnicos objetivos.

### Acceso a Internet
- Estado actual: DESACTIVADO
- Estado futuro: ACTIVABLE
- Condición de activación:
  - Core completamente estable
  - Arquitectura sin dependencias legacy
  - Confirmación explícita del usuario
- Uso futuro:
  - Consultas bajo demanda
  - Sin ejecución automática
  - Resultados filtrados y auditables

### Evaluación del equipo (hardware awareness)
- NOVA podrá evaluar localmente:
  - CPU
  - RAM
  - GPU
  - Dispositivos de audio
  - Sistema operativo
- Esta evaluación será local y no se enviará información externa.
- Servirá como base para decisiones futuras.

### Voz, escucha y avatar
- Estado actual: NO IMPLEMENTADO
- Estado futuro: IMPLEMENTABLE
- Condición:
  - NOVA debe poder evaluar el hardware disponible
  - NOVA debe determinar qué modelos son viables
  - El usuario debe autorizar explícitamente cada capacidad
- Capacidades futuras posibles:
  - Voz sintética local
  - Clonación de voz autorizada
  - Escucha mediante STT local
  - Avatar visual como capa de presentación
- NOVA podrá proponer estas capacidades, pero nunca activarlas sin confirmación humana.

---

## PROBLEMAS RESUELTOS (NO REABRIR)

- Repetición infinita de comandos
- Logs tipo "Usuario / Respuesta"
- Router causando loops
- InternetLayer rompiendo flujo
- LLaMA devolviendo texto largo
- Executor duplicando mensajes
- CLI reinyectando input
- Conflictos entre arquitectura vieja y nueva

---

## TRABAJO PENDIENTE

Pendiente de implementar:
1. Correcciones iterativas con preview/diff
2. Edición por secciones
3. Estructuras avanzadas (src/, tests/)
4. Definición formal de “NOVA al 100%”
5. Activación de Internet (cuando se cumplan condiciones)

---

## REGLA DE ORO

Este archivo define el estado real, válido y autorizado del proyecto NOVA.  
Si cualquier sugerencia futura contradice este bloque, la sugerencia es incorrecta.

---

## USO EN NUEVOS CHATS

Al iniciar un nuevo chat:
1. Pegar este archivo completo.
2. Indicar explícitamente:
   “Este es el estado válido del proyecto NOVA. Continúa desde aquí.”

No es necesario explicar nada más.
