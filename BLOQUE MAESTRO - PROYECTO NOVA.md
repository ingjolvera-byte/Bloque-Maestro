# BLOQUE MAESTRO UNIFICADO v3.1-U

## PROYECTO NOVA IA

IA OFFLINE (LLAMA) + GUI CORPORATIVA + INTERNET CONTROLADO

Estado: **CONGELADO ABSOLUTO**
Fecha: 2025-12-26
Dependencia base: Bloque Maestro v2 (NÚCLEO INMUTABLE)

---

## 1. PRINCIPIO SUPREMO

* El **Núcleo v2 no se modifica**.
* Todo lo definido aquí se construye **encima** del núcleo.
* Si una decisión rompe el núcleo, **no se implementa**.
* Este documento sustituye y unifica todos los bloques anteriores.

---

## 2. OBJETIVO GLOBAL

Convertir NOVA en un **producto enterprise real**, previo a empaquetado:

* IA offline de alto nivel (LLAMA)
* Arquitectura cognitiva gobernante
* CLI profesional
* GUI corporativa premium (fase posterior)
* Acceso a internet **limitado, explícito y auditable**

No incluye:

* Monetización
* Licenciamiento
* Distribución

---

## 3. CONCEPTO FUNDAMENTAL

* NOVA **no es un chatbot**.
* NOVA es un **sistema cognitivo híbrido**.
* El **cerebro es offline**.
* Internet es **auxiliar**, nunca central.
* Los modelos **no gobiernan**: la arquitectura gobierna.

---

## 4. CEREBRO OFFLINE (IA)

### Modelo base

* Familia: **LLAMA**
* Ejecución: **local / offline**
* Backend: `llama.cpp`

### Identidad lógica (inmutable)

```
brain.llama.primary
```

### Resolución física actual

```
D:\NOVA\NOVA_IA\models\llama3\Llama3.1-8B_Instruct-q4.gguf
```

Reglas:

* El sistema **nunca referencia modelos por filename**.
* El filename es intercambiable.
* El ID lógico es estable.

---

## 5. POLÍTICA DE INTERNET

Internet:

* No es dependencia
* No es automática
* No es silenciosa

### Usos permitidos

* Búsquedas públicas
* Descarga de archivos
* Verificación de versiones
* Consulta de documentación

### Usos prohibidos

* Telemetría
* Envío de datos sin permiso
* Ejecución remota
* Conexiones persistentes

### Reglas obligatorias

* Módulo dedicado
* Logging completo
* Consentimiento explícito
* Usuario puede aislar totalmente el sistema

---

## 6. ARQUITECTURA COGNITIVA (CAPAS)

Capas definidas y cerradas:

1. Interpreter
2. Planner
3. Router Cognitivo
4. Executor
5. Internet Layer
6. Responder

Cada capa:

* Tiene contrato formal
* Es reemplazable
* No tiene efectos colaterales

---

## 7. MÁQUINA DE ESTADOS GLOBAL

Estados válidos:

* IDLE
* INTERPRETING
* PLANNING
* ROUTING
* INTERNET_PENDING
* INTERNET_EXECUTING
* EXECUTING
* RESPONDING
* ERROR

Transiciones explícitas.
Transiciones implícitas: **prohibidas**.

---

## 8. POLÍTICA DE DECISIÓN DE INTERNET

Gobernada por el **Planner** mediante tabla cerrada:

Variables:

* requires_internet
* system_isolation
* permission_mode
* risk_level

Resultados posibles:

* CORE_ONLY
* INTERNET_REQUIRED
* CONFIRMATION_REQUIRED
* BLOCKED

No existe escalado automático de permisos.

---

## 9. MEMORIA

### Tipos

1. Memoria de sesión (volátil)
2. Memoria persistente (controlada por usuario)
3. Memoria técnica del sistema

Reglas:

* No hay auto-guardado
* No hay persistencia implícita
* Usuario controla qué se guarda

---

## 10. LOGGING Y AUDITORÍA

Tipos de log:

* Cognitivo
* Ejecución
* Internet
* Memoria

Formato:

* Estructurado
* Local
* Auditable
* Sin envío externo

---

## 11. ORDEN OBLIGATORIO DE TRABAJO

1. Arquitectura de IA (COMPLETADO)
2. Implementación CLI (EN CURSO)
3. Integración de Internet
4. Diseño GUI premium
5. Implementación GUI
6. Empaquetado

Cambiar el orden **rompe el producto**.

---

## 12. ESTRUCTURA OFICIAL DEL PROYECTO

Raíz fija:

```
D:\NOVA\NOVA_IA\
```

Estructura actual:

```
D:\NOVA\NOVA_IA\
├─ cli\
│  ├─ __init__.py
│  ├─ main.py
│  ├─ cli_loop.py
│  └─ cli_commands.py
│
├─ core\
│  ├─ __init__.py
│  ├─ enums.py
│  └─ state_machine.py
│
├─ models\
│  ├─ __init__.py
│  ├─ base_model.py
│  ├─ llama_cpp_model.py
│  ├─ model_manager.py
│  └─ llama3\
│     └─ Llama3.1-8B_Instruct-q4.gguf
│
├─ memory\
│  ├─ __init__.py
│  ├─ session_memory.py
│  ├─ persistent_memory.py
│  └─ system_memory.py
│
├─ logging\
│  ├─ __init__.py
│  └─ audit_logger.py
│
└─ main.py
```

---

## 13. CLI (EN CURSO)

Principios:

* Determinista
* Observable
* Sin magia

Comandos base:

* status
* load brain
* unload brain
* run
* exit

Estados visibles al usuario.

---

## 14. REGLA DE CONTINUIDAD

* Este documento es la **única fuente de verdad**.
* Cualquier cambio requiere:

  * Nuevo bloque maestro versionado
  * Documentación explícita

---

## FIN DEL BLOQUE MAESTRO UNIFICADO v3.1-U
