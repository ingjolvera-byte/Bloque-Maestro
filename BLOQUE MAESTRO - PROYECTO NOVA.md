# BLOQUE MAESTRO OFICIAL – PROYECTO NOVA IA

**Versión:** Base Estable v1.0
**Estado:** Saneamiento previo a corrección y empaquetado

---

## PRINCIPIOS ABSOLUTOS (NO NEGOCIABLES)

1. NOVA es 100% offline.
2. NOVA no usa web ni servidores externos.
3. NOVA no descarga ni ejecuta nada peligroso automáticamente.
4. NOVA no toca archivos críticos de Windows.
5. Todo lo que NOVA crea va únicamente a la carpeta `sandbox`.
6. No se usan rutas mágicas ni módulos que no existan físicamente.
7. No se adivina código ni se hacen parches parciales.
8. Si algo no está definido aquí, no se usa.
9. El usuario no tiene que “buscar dónde va algo”.
10. El sistema debe funcionar igual en CLI y GUI.

---

## OBJETIVO ACTUAL

Dejar el núcleo de NOVA completamente estable y alineado antes de crear nuevas funciones, mejorar la GUI o empaquetar en EXE.

---

## ESTRUCTURA OFICIAL DEL PROYECTO (NO CAMBIAR)

```
NOVA_IA/
│
├── core/
│   ├── nova_executor.py
│   ├── response_manager.py
│   ├── capability_manager.py
│   └── __init__.py
│
├── memory/
│   ├── memory_store.py
│   ├── data/
│   │   └── memory.json
│   └── __init__.py
│
├── modules/
│   ├── translate/
│   ├── hardware/
│   ├── filesystem/
│   ├── dependencies/
│   ├── updates/
│   ├── create/
│   ├── image/
│   ├── audio/
│   ├── models/
│   └── __init__.py
│
├── gui/
│   └── gui_nova.py
│
├── pipeline/
│
├── sandbox/
│
├── logs/
│
├── tools/
│
├── main.py
└── updater.py
```

---

## RESPONSABILIDAD DE CADA PARTE

### core

Coordina el sistema. Decide qué hacer con el texto del usuario. Llama a los módulos correctos. No ejecuta lógica pesada. No crea archivos. No usa GUI.

### memory

Guarda y devuelve información persistente. No conoce al core. No conoce a la GUI. No importa módulos externos.

### modules

Cada módulo hace una sola tarea específica (traducir, hardware, archivos, etc.). No se comunican entre sí. No conocen al core ni a la GUI.

### gui

Interfaz gráfica. Solo envía texto al executor y muestra el resultado. No ejecuta lógica. No importa módulos.

### sandbox

Único lugar donde NOVA puede crear archivos, proyectos, software, imágenes o audio.

---

## ARCHIVOS CONGELADOS (BASE DEL SISTEMA)

Estos archivos se corrigen primero y luego no se modifican sin control:

* `core/nova_executor.py`
* `core/response_manager.py`
* `memory/memory_store.py`

---

## REGLAS DE IMPORTS (LENGUAJE SIMPLE)

* Si un archivo no existe, no se importa.
* Si una clase no existe, no se usa.
* `core` puede importar `modules` y `memory`.
* `modules` no pueden importar `core`.
* `gui` solo puede importar `core`.
* `memory` no importa `core`.

---

## MÉTODO OFICIAL DEL EXECUTOR

El único método público del sistema es:

```
NovaExecutor.run(texto)
```

No existen ni se usarán:

* execute
* process
* handle
* otros nombres

---

## FORMA DE TRABAJO ACORDADA

* El usuario pega el archivo completo.
* El asistente devuelve el archivo completo corregido.
* No se dan instrucciones de “busca esto” o “cambia esta línea”.
* Se corrige un archivo a la vez.
* Se resuelve un problema a la vez.

---

## ESTADO ACTUAL REAL

* La GUI abre.
* La memoria funciona.
* El executor ejecuta acciones.
* Los errores actuales son solo de alineación de nombres e imports.
* No hay pérdida de código.
* No se empieza de cero.

---

## PRÓXIMO PASO EN EL NUEVO CHAT

1. Pegar `core/nova_executor.py`.
2. Corregirlo y congelarlo.
3. Pegar `core/response_manager.py`.
4. Congelarlo.
5. Pegar `memory/memory_store.py`.
6. Confirmar estabilidad.
7. Crear Bloque Maestro v2.
8. Continuar con GUI, IA y empaquetado.

---

**FIN DEL BLOQUE MAESTRO**
