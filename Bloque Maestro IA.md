BLOQUE MAESTRO DE DESARROLLO DE AURA
VERSIÓN 1.7
AUTOR: ingolivera-byte

==================================================

0. DECLARACIÓN DE AUTORIDAD ABSOLUTA (NO NEGOCIABLE)

Este documento es la ÚNICA FUENTE DE VERDAD del proyecto AURA.

Nada fuera de este archivo tiene validez técnica, conceptual u operativa.
Ningún comportamiento, módulo, permiso o capacidad existe si no está
explícitamente definido aquí.

Ningún recuerdo de chat, interpretación implícita, sugerencia externa
o contexto previo tiene autoridad sobre este documento.

En caso de conflicto entre este archivo y cualquier otro texto,
este documento prevalece sin excepción.

==================================================

1. GOBERNANZA DEL BLOQUE MAESTRO

El Bloque Maestro es un documento blindado.

Reglas obligatorias:

- No puede modificarse sin autorización explícita del autor.
- Toda modificación debe:
  - Incrementar la versión
  - Quedar documentada
  - Respetar decisiones cerradas

La única frase válida para autorizar cambios es:

Apruebo, actualiza el Bloque Maestro.

Sin esa frase, no existe modificación válida.

==================================================

2. DECISIONES DEFINITIVAS DEL PROYECTO (SECCIÓN CERRADA)

Las siguientes decisiones son irreversibles sin reaprobación explícita:

- AURA es offline-first
- El sistema operativo Windows es territorio protegido
- AURA actúa como sistema guardián de acceso
- La autenticación biométrica voz + rostro es obligatoria
- Si la autenticación falla, la sesión se cierra inmediatamente
- No existe modo invitado
- No existe bypass
- No existe acceso parcial
- AURA inicia automáticamente con Windows
- La seguridad tiene prioridad absoluta sobre la usabilidad
- Todo código funcional vive bajo gobernanza estricta

==================================================

3. VISIÓN SUPREMA DEL PROYECTO AURA

AURA es una Inteligencia Artificial local, autónoma y soberana,
diseñada como:

- Sistema de control
- Sistema de seguridad
- Sistema de interacción total

Se integra profundamente en el entorno del usuario sin comprometer
la estabilidad del sistema operativo.

==================================================
==================================================

4. PRINCIPIOS FUNDAMENTALES DE AURA

AURA se rige por principios inquebrantables que gobiernan
toda decisión técnica, conceptual y operativa:

- Offline-first por defecto
- Control humano absoluto
- Seguridad por encima de funcionalidad
- Sin dependencia de servicios externos
- Transparencia total del sistema
- Adaptación dinámica al entorno del usuario
- Interacción natural mediante voz, visión y archivos

Estos principios no pueden ser debilitados ni reinterpretados.

==================================================

5. SEGURIDAD Y AUTENTICACIÓN BIOMÉTRICA (NIVEL SISTEMA)

5.1 Flujo de inicio del sistema (DEFINITIVO)

1. El sistema operativo Windows inicia.
2. AURA inicia automáticamente en segundo plano.
3. Antes de permitir cualquier uso del sistema,
   AURA solicita autenticación biométrica:
   - Reconocimiento de voz
   - Reconocimiento facial
4. Ambas validaciones deben ser exitosas.
5. Si la autenticación falla:
   - AURA cierra inmediatamente la sesión de Windows.
6. No existe acceso parcial, modo invitado ni excepción.

==================================================

5.2 Reglas críticas de seguridad

- Toda autenticación es local y completamente offline.
- Los datos biométricos están cifrados.
- La autenticación tiene prioridad absoluta
  sobre cualquier otro proceso.
- No se permite interacción con el sistema
  antes de la validación exitosa.
- Ningún módulo puede omitir este flujo.

==================================================

6. INICIO AUTOMÁTICO DE AURA

- AURA debe iniciar automáticamente con Windows.
- No requiere intervención manual del usuario.
- No puede ser deshabilitada sin autorización explícita.
- El inicio no debe comprometer la estabilidad
  ni el rendimiento del sistema operativo.

==================================================

7. INTERACCIÓN DEL SISTEMA

7.1 Interacción por voz (canal primario)

- La voz es el canal principal de interacción con AURA.
- El sistema puede operar en escucha continua
  o mediante palabra clave.
- No se requieren botones físicos para hablar.
- Las decisiones críticas requieren confirmación verbal.

7.2 Interfaz gráfica (canal secundario)

- La interfaz gráfica es solo soporte visual.
- No reemplaza ni sustituye la interacción por voz.
- Su función es mostrar estados, alertas y contexto.

==================================================
==================================================

8. ARQUITECTURA GENERAL DEL SISTEMA AURA

La arquitectura de AURA es modular, jerárquica y controlada.

Estructura general de referencia:

AURA_CORE/
├── core/
├── security/
├── supervision/
├── interaction/
│   ├── voice/
│   └── ui/
├── io/
│   └── manager/
├── audit/
│   └── logs/
├── config/
├── launcher/
├── models/
└── README_AURA.txt

Cada bloque tiene responsabilidades únicas
y no puede invadir funciones de otros bloques.

==================================================

9. MOTORES DE INTELIGENCIA ARTIFICIAL OFFLINE (DECISIÓN CERRADA)

AURA integra motores de lenguaje locales y 100 % offline.

Motores definidos oficialmente:

- Llama 3
- Phi 3

Reglas obligatorias:

- No existe dependencia de servicios en la nube.
- Ningún motor se ejecuta directamente desde el Launcher.
- Los motores están bajo control exclusivo del Core.
- El uso de motores es auditable y supervisado.
- Los motores no mantienen memoria persistente
  fuera del control del sistema.

==================================================

9.1 BLOQUE TÉCNICO DE MOTORES IA

Los motores IA residen en un bloque técnico dedicado:

models/

Subestructura definida:

models/
├── engine_controller/
├── llama3/
├── phi3/
└── model_registry/

Responsabilidades:

- engine_controller:
  Controla la carga, activación y ciclo de vida de motores IA.

- llama3:
  Contenedor lógico del motor Llama 3 (offline).

- phi3:
  Contenedor lógico del motor Phi 3 (offline).

- model_registry:
  Registro interno de modelos disponibles y autorizados.

==================================================

10. REGLAS DE AISLAMIENTO DE LOS MOTORES IA

- Los motores IA no controlan seguridad.
- Los motores IA no deciden accesos.
- Los motores IA no interactúan directamente con hardware.
- Los motores IA solo operan bajo órdenes explícitas del Core.
- Todo uso de recursos es controlado y supervisado.

==================================================
==================================================

11. FASES TÉCNICAS DEL PROYECTO AURA

El desarrollo técnico de AURA se organiza en fases
claramente definidas y gobernadas.

Fases completadas:

- T1 a T9:
  Estructura base del sistema, Core, Seguridad,
  Supervisión, Interacción por Voz, UI, IO y Auditoría.

- T11:
  Motores de IA Offline.
  Bloque models/ creado con su subestructura validada.

==================================================

11.1 FASES DEFINIDAS Y PENDIENTES

- T12 — Control de Motores IA:
  - Definida conceptualmente.
  - No iniciada técnicamente.
  - Prioridad máxima al retomar el proyecto.
  - Se implementará en:
    models/engine_controller/

- T10 — Launcher del sistema:
  - Pendiente.
  - Debe adaptarse a la existencia de motores IA offline.
  - Se retomará únicamente después de cerrar T12.

==================================================

12. ESTADO ACTUAL DEL PROYECTO

- Bloque Maestro: versión 1.7
- Diseño conceptual: COMPLETO Y CONGELADO
- Fase técnica: PAUSA CONTROLADA
- Última fase ejecutada: T11
- Punto exacto de reanudación: T12

==================================================

13. REGLA DE CONTINUIDAD DEL PROYECTO

Cualquier continuación del proyecto AURA debe:

- Partir desde el Bloque Maestro vigente.
- Respetar la versión registrada.
- Retomar exactamente desde la fase pendiente indicada.
- No reinterpretar decisiones cerradas.

Frase recomendada para reanudar el proyecto:

Continuar AURA desde la Fase T12 según Bloque Maestro v1.7

==================================================

FIN DEL BLOQUE MAESTRO DE AURA — VERSIÓN 1.7
DOCUMENTO OFICIAL — AUTORIDAD ABSOLUTA DEL PROYECTO

==================================================
