# 🧠 BLOQUE MAESTRO — PROYECTO NOVA

## ESTADO GENERAL

Proyecto: NOVA
Tipo: IA local (Personal + Empresa)
Sistema: Windows
Fuente de verdad: Este Bloque Maestro
Regla suprema: Lo funcional NO se toca

---

## ⚠️ SECCIÓN CRÍTICA — CÓMO DEBE USARSE ESTE BLOQUE (LECTURA OBLIGATORIA)

Este documento NO es solo documentación.
Este documento ES el contrato, la memoria y la única referencia válida del proyecto.

### Reglas absolutas de uso (ACLARADAS Y CORREGIDAS)

1. **Este archivo es indivisible**

   * No se separa en partes
   * No se resume
   * No se reescribe por secciones
   * Se copia y pega COMPLETO

2. **Todo lo importante debe vivir aquí**

   * Decisiones técnicas
   * Código funcional FINAL
   * Cambios válidos y aprendidos
   * Reglas corregidas
     Si algo NO está aquí, **no existe**.

3. **Código funcional**

   * Siempre existe **UN SOLO CÓDIGO VÁLIDO por fase**
   * No se aplican parches incrementales en chat
   * Todo cambio implica **reemplazo completo del archivo**

4. **Actualización del bloque**

   * El bloque se ACTUALIZA, no se versiona
   * Solo existe UNA versión válida: la última funcional
   * Versiones rotas o intermedias NO se documentan

5. **Fases**

   * Cada fase tiene estado: Iniciada / En progreso / Funcional / Congelada
   * Una fase Congelada NO se toca
   * Extender funcionalidad SOLO está permitido mientras la fase esté activa

6. **Progresión**

   * No se saltan fases
   * No se avanza si el comportamiento no está comprendido
   * Se congela una fase solo cuando:

     * el comportamiento es estable
     * el comportamiento es comprendido

7. **Instrucciones operativas (CLAVE)**

   * Siempre **UN SOLO OBJETIVO por mensaje**
   * Nunca mezclar:

     * debugging
     * diseño
     * optimización
   * Si hay confusión, **se detiene el avance y se aclaran reglas**

8. **Regla anti-confusión (nueva)**

   * Si un comportamiento es *esperado* (ej. latencia en CPU),
     NO se trata como error
   * Primero se explica el comportamiento
   * Luego se decide si se optimiza o se acepta

Estas reglas existen para evitar exactamente:

* pérdida de avances
* loops de corrección
* cambios contradictorios
* desgaste innecesario

Si estas reglas no se respetan, el proyecto se detiene.

---

## ENTORNO DEL EQUIPO

Sistema Operativo:

* Windows 11 (64 bits)

Hardware:

* CPU: AMD Ryzen 5 7535HS
* RAM actual: 16 GB
* RAM planificada: 40 GB → 64 GB
* GPU: Integrada (CPU inference)
* Audio:

  * Micrófono USB
  * Auriculares

Python:

* Versión: 3.11.x
* Entorno virtual: .venv
* Librerías instaladas: pip list confirmado
* Empaquetado disponible: PyInstaller

---

## ESTRUCTURA DEL PROYECTO (BASE LIMPIA)

D:\aura
├── .venv
└── models\

---

## MODELOS IA

models
├── llama3
│   └── Meta-Llama-3.1-8B-Instruct-Q4_0.gguf
└── vosk-es\

Modelo principal:

* Meta-Llama-3.1-8B-Instruct-Q4_0.gguf
* Uso: Núcleo cognitivo
* Modo: Offline-first

STT:

* VOSK (reservado para fases futuras)

---

## CONECTIVIDAD

Modo principal: Offline
Acceso a internet: Sí

Restricciones:

* No enviar información privada
* No telemetría
* No exfiltración de datos

---

## IDIOMA

* Español + Inglés
* Responde en el idioma en que se le hable

---

## SEGURIDAD

Nivel de permisos: Administrador

Restricciones:

* Sin acceso a componentes críticos de Windows
* Sin acciones destructivas
* Sin modificar registro crítico

Toda acción sensible requiere confirmación explícita.

---

## INTERFAZ

Tipo: Aplicación nativa de Windows

Prohibido:

* Web
* Navegador
* Flask / servidores locales

Permitido:

* Consola (fase inicial)
* GUI Windows nativa (fases posteriores)

---

## PERSONALIDAD DE NOVA

Tipo: Mixta

* Creativa para diseño y desarrollo
* Prudente para sistema y datos

Referencia conceptual: IRON MAN + TRON

---

## FASES DEL PROYECTO (ORDEN OBLIGATORIO)

FASE 1 — Núcleo Cerebral
FASE 2 — Voz
Estado: Funcional → Congelada

FASE 3 — Interfaz Windows

FASE 4 — Memoria
FASE 5 — Acceso Controlado al Sistema
FASE 6 — Integraciones
FASE 7 — Auto-actualización
FASE 8 — Empaquetado

---

# 🔹 FASE 1 — NÚCLEO CEREBRAL

**Estado:** Iniciada

## Objetivo

Construir un núcleo cognitivo local capaz de:

* Cargar el modelo LLaMA 3.1 GGUF
* Mantener conversación por consola
* Operar 100% offline
* Ser estable y reproducible

Este núcleo será la base de TODO el sistema.
Si esta fase falla, el proyecto no continúa.

---

## Alcance

Incluye:

* Inicialización del entorno
* Carga del modelo GGUF
* Bucle de conversación
* Manejo básico de errores

Excluye (futuras fases):

* Voz
* GUI
* Memoria persistente
* Acciones de sistema

---

## DECISIONES CLAVE

* Motor: llama-cpp-python
* Inferencia: CPU
* Interfaz: Consola
* Arquitectura: Script único

---

## DEPENDENCIAS

Instalar (dentro de .venv):

* llama-cpp-python

---

## CÓDIGO FUNCIONAL — FASE 1

⚠️ ESTE ES EL ÚNICO CÓDIGO VÁLIDO PARA LA FASE 1

```python
import sys
from llama_cpp import Llama
import pyttsx3

MODEL_PATH = "models/llama3/Meta-Llama-3.1-8B-Instruct-Q4_0.gguf"

# Inicializar modelo
llm = Llama(
    model_path=MODEL_PATH,
    n_ctx=4096,
    n_threads=8,
    verbose=False
)

# Inicializar motor de voz (SAPI5 en Windows)
tts = pyttsx3.init()
tts.setProperty("rate", 170)
tts.setProperty("volume", 1.0)

print("NOVA — Núcleo Cerebral iniciado. Escribe 'salir' para terminar.
")

while True:
    try:
        user_input = input("Tú: ")

        if user_input.lower() in ["salir", "exit", "quit"]:
            print("NOVA: Apagando núcleo cerebral.")
            break

        response = llm(
            f"<|user|>
{user_input}<|end|>
<|assistant|>",
            max_tokens=512,
            stop=["<|end|>"]
        )

        answer = response["choices"][0]["text"].strip()
        print("NOVA:", answer, "
")

        # Forzar lectura completa en cada turno
        tts.stop()              # limpia cola previa
        tts.say(answer)         # encola texto completo
        tts.runAndWait()        # bloquea hasta terminar

    except KeyboardInterrupt:
        print("
NOVA: Interrupción manual detectada. Apagando núcleo.")
        sys.exit(0)

    except Exception as e:
        print("NOVA: Error:", str(e))
```

---

## CRITERIOS DE VALIDACIÓN

La Fase 1 se considera **FUNCIONAL** cuando:

* El modelo carga sin error
* Responde coherentemente por consola
* No se cuelga tras múltiples prompts

---

## BLOQUEO

Una vez validada, esta fase se marca como:
**Estado: Funcional → Congelada**

A partir de ese momento:

* Este código NO se toca
* Cualquier mejora va a otra fase

---

## NOTA FINAL DE FASE

Este núcleo es el corazón de NOVA.
Todo lo demás depende de que esto sea sólido.
