# ARCHIVO DE FASES — CORRECCIÓN Y ARMONIZACIÓN OPERATIVA

## 0. Principio rector
El Archivo de Fases **no define arquitectura ni autoridad**.  
Su única función es **ordenar el trabajo en el tiempo** conforme al Bloque Maestro.

Ninguna fase puede:
- introducir jerarquías
- asumir estructuras implícitas
- cerrar decisiones no definidas en el Bloque Maestro

Si existe conflicto, **manda siempre el Bloque Maestro**.

---

## 1. Naturaleza de las fases
Las fases en AURA son:

- Instrumentos de organización
- No estados rígidos del sistema
- No capas arquitectónicas

Una fase puede:
- solaparse con otra
- revisarse
- reabrirse
- ejecutarse parcialmente

Nada se considera “cerrado” salvo confirmación explícita del usuario.

---

## 2. Estado real de las fases (corrección)

### FASE 0 — Fundamentos
**Estado:** Implícita / no cerrada  

Contenido válido:
- Definición conceptual inicial
- Bloque Maestro
- Contratos mínimos
- Principios operativos

Corrección:
- FASE 0 **no se considera completada**
- Sirve como base permanente de referencia

---

### FASE 1 — Diseño estructural
**Estado:** Parcial / revisable  

Contenido válido:
- Propuesta de módulos
- Flujos lógicos
- Diagramas conceptuales

Corrección:
- Todo lo aquí descrito es **provisional**
- No implica jerarquía ejecutiva
- No implica implementación real

---

### FASE 2 — Implementación inicial
**Estado:** NO INICIADA (formalmente)

Corrección explícita:
- Ningún código previo marca el inicio formal de la fase
- El código existente se considera:
  - prototipo
  - prueba de flujo
  - exploración técnica

La FASE 2 solo inicia cuando el usuario lo confirme explícitamente.

---

### FASE 3 — Inteligencia funcional
**Estado:** No iniciada  

Contenido previsto (no obligatorio):
- Modelos
- Razonamiento
- Memoria
- Aprendizaje

Corrección:
- No se asume dependencia directa con fases anteriores
- Puede iniciarse parcialmente si el usuario lo decide

---

### FASE 4 — Supervisión y control
**Estado:** No iniciada  

Contenido previsto:
- Supervisión
- Autocontrol
- Metarazonamiento

Corrección:
- No se asume como “fase final”
- Puede redefinirse completamente

---

## 3. Prohibición de lectura secuencial obligatoria
Las fases **no deben leerse como un pipeline rígido**.

No existe la obligación de:
- terminar una fase para empezar otra
- completar una fase para validar el sistema

El orden sirve solo como **guía**, no como restricción.

---

## 4. Relación con el Bloque Maestro
El Archivo de Fases:

- Nunca redefine conceptos del Bloque Maestro
- Nunca corrige arquitectura
- Nunca introduce autoridad

Si un texto de fases contradice al Bloque Maestro:
- se considera inválido
- debe corregirse
- no genera ambigüedad

---

## 5. Regla de inicio y cierre de fases
- Una fase inicia solo cuando el usuario lo declara
- Una fase se cierra solo cuando el usuario lo confirma
- El silencio **no implica avance**
- El código por sí solo **no marca progreso formal**

---

## 6. Estado tras esta corrección
Después de aplicar este bloque:

- El Archivo de Fases queda alineado con el Bloque 0
- No induce suposiciones
- No fuerza interpretaciones
- No bloquea el avance

El proyecto queda en un estado **ordenado pero flexible**.

FIN DEL ARCHIVO DE FASES — CORRECCIÓN OPERATIVA
