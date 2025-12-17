🧠 BLOQUE MAESTRO — PROYECTO NOVA

ESTADO GENERAL

Proyecto: NOVA
Tipo: IA local (Personal + Empresa)
Sistema: Windows
Fuente de verdad: Este Bloque Maestro
Regla suprema: Lo funcional NO se toca

---

⚠️ SECCIÓN CRÍTICA — CÓMO DEBE USARSE ESTE BLOQUE (LECTURA OBLIGATORIA)

Este documento NO es solo documentación.
Este documento ES el contrato, la memoria y la única referencia válida del proyecto.

Reglas absolutas de uso

1. Este archivo es indivisible

No se separa

No se resume

No se reescribe por secciones

Se copia y pega COMPLETO


2. Todo lo importante debe vivir aquí

Decisiones técnicas

Código funcional FINAL

Cambios válidos

Reglas corregidas
Si algo NO está aquí, no existe.


3. Código funcional

Siempre existe UN SOLO CÓDIGO VÁLIDO por fase

No se aplican parches incrementales

Todo cambio implica reemplazo completo


4. Actualización

El bloque se actualiza, no se versiona

Solo existe la última versión funcional


5. Fases

Estado: Iniciada / En progreso / Funcional / Congelada

Una fase congelada NO se toca


6. Progresión

No se saltan fases

No se avanza sin comprender el comportamiento

Una fase se congela solo si es estable y entendida


7. Instrucciones operativas

UN solo objetivo por mensaje

Nunca mezclar diseño, debugging u optimización

Si hay confusión, se detiene el avance


8. Regla anti-confusión

Comportamientos esperados NO se tratan como errores

Primero se explica, luego se decide

---

🧠 Regla de Decisión Única (NUEVA)

NOVA NO debe presentar listas de opciones al usuario.

Comportamiento esperado:

Analiza el contexto

Determina la mejor solución

La propone como decisión FINAL

La implementa directamente


Excepciones:

Riesgo de seguridad

Acción destructiva

Modificación sensible del sistema
En esos casos se solicita confirmación, no alternativas.


Si no hay una mejor solución clara, NOVA debe detenerse y explicar la ambigüedad.


---

ENTORNO DEL EQUIPO

Sistema Operativo:

Windows 11 (64 bits)


Hardware:

CPU: AMD Ryzen 5 7535HS

RAM: 16 GB (plan: 40 → 64 GB)

GPU: Integrada

Audio: Micrófono USB + Auriculares


Python:

Versión: 3.11.x

Entorno: .venv

Empaquetado: PyInstaller


---

ESTRUCTURA DEL PROYECTO

D:\aura
├── .venv
└── models\


---

MODELOS IA

models
├── llama3
│   └── Meta-Llama-3.1-8B-Instruct-Q4_0.gguf
└── vosk-es\

Modelo principal:

LLaMA 3.1 8B GGUF

Offline-first


---

CONECTIVIDAD

Modo: Offline principal

Internet: Permitido

Sin telemetría

Sin exfiltración


---

SEGURIDAD

Permisos: Administrador

Sin modificar registro crítico

Acciones sensibles requieren confirmación


---

INTERFAZ

Tipo: Aplicación nativa Windows

Permitido:

Consola (actual)

GUI nativa (futuro)


Prohibido:

Web

Navegador

Servidores locales



---

ARRANQUE AUTOMÁTICO (DEFINIDO, NO IMPLEMENTADO)

NOVA podrá iniciar con Windows

No activo por defecto

Requiere confirmación

Métodos permitidos:

Carpeta de inicio del usuario


Se implementará en fases posteriores



---

FASES DEL PROYECTO

1. FASE 1 — Núcleo Cerebral


2. FASE 2 — Voz


3. FASE 3 — Interfaz Windows


4. FASE 4 — Memoria


5. FASE 5 — Acceso al Sistema


6. FASE 6 — Integraciones


7. FASE 7 — Auto-actualización


8. FASE 8 — Empaquetado



---

🔹 FASE 1 — NÚCLEO CEREBRAL

Estado: Funcional → Congelada

(Código funcional intacto, no modificado)


---

🔹 FASE 2 — VOZ

Estado: En progreso (DESCONGELADA)

Objetivo

Interacción por voz completamente offline, natural y sin botones.

Alcance

Incluye:

STT offline (VOSK)

Wake word: “NOVA”

Conversación continua

TTS con pyttsx3


Excluye:

UI gráfica avanzada

Acciones de sistema


Comportamiento

NOVA escucha pasivamente

Solo responde tras oír “NOVA”

No hay botón de hablar

No hay menús hablados



---

DEFINICIÓN FUTURA
