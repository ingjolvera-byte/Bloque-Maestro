# 🧠 BLOQUE MAESTRO DEFINITIVO — PROYECTO NOVA

## 📌 Visión General
NOVA es una **IA local, offline, acelerada por GPU**, diseñada como un **cerebro conversacional y lógico**.  
Opera sin conexión a internet y puede ampliarse mediante **módulos externos**, manteniendo siempre el control humano y la seguridad del sistema.

NOVA **NO ejecuta acciones del sistema operativo por sí sola**.  
Para realizar acciones reales (crear archivos, usar programas, compilar, instalar, etc.) requiere un **Agente Ejecutor externo**.

---

## 🟢 FASES COMPLETADAS (DESDE FASE 1)

### 🟢 FASE 1 — Diseño y Arquitectura Base
**Estado:** COMPLETA  
- Definición de la visión del proyecto  
- Arquitectura modular  
- Separación core / engine / UI  
- Decisión de IA local y offline  

---

### 🟢 FASE 2 — Selección y Validación del Modelo
**Estado:** COMPLETA  
- Uso de modelos GGUF  
- LLaMA Instruct local  
- Pruebas en CPU y GPU  
- Contexto estable  

---

### 🟢 FASE 3 — Motor de Inferencia (`nova_engine`)
**Estado:** COMPLETA (LIMPIA Y ESTABLE)  
- Prompt del sistema único  
- Respuesta directa (1 input → 1 output)  
- Uso correcto de GPU (CUDA)  
- Sin bucles ni divagaciones  

---

### 🟢 FASE 4 — Núcleo Lógico (`nova_core`)
**Estado:** COMPLETA  
- Pasarela entre usuario y motor  
- Sin conversación fantasma  
- Sin auto-ejecución de acciones  
- Texto limpio y estable  

---

### 🟢 FASE 5 — CLI / Interfaz Base
**Estado:** COMPLETA  
- Interacción desde terminal  
- Manejo de salida (`exit`, `quit`)  
- Control básico de errores  

---

### 🟢 FASE 6 — Memoria / Estado Controlado
**Estado:** COMPLETA / CONGELADA  
- Memoria explícita  
- Sin auto-modificación  
- Determinismo controlado  

---

### 🟢 FASE 7 — UI / UX Básica
**Estado:** COMPLETA / CONGELADA  
- Interfaz funcional  
- No crítica para el núcleo  

---

### 🟢 FASE 8 — Router Lógico
**Estado:** COMPLETA / CONGELADA  
- Clasificación de intención  
- Separación entre diálogo y acciones  
- Sin ejecución real  

---

### 🟢 FASE 9 — Preferencias y Criterios
**Estado:** COMPLETA / CONGELADA  
- Preferencias persistentes  
- Reglas de comportamiento  

---

### 🟢 FASE 10 — Control de Prompts
**Estado:** COMPLETA / CONGELADA  
- Prompt del sistema estable  
- Sin inyección caótica  
- Sin alucinaciones funcionales  

---

### 🟢 FASE 11 — Estabilidad y Validación
**Estado:** COMPLETA  
- Pruebas prolongadas  
- Respuestas coherentes  
- Rendimiento estable  

---

### 🟢 FASE 12 — Consolidación del Núcleo
**Estado:** COMPLETA  
- Código limpio  
- Core y engine separados  
- Proyecto estable  

---

## ❌ FASES ELIMINADAS VOLUNTARIAMENTE

### 🔴 FASE 13 — Voz (TTS / STT)
**Estado:** ELIMINADA  
- Inestabilidad  
- Latencia  
- No esencial para el núcleo  

---

### 🔴 FASE 14 — Automatismos Prematuros
**Estado:** ELIMINADA  
- Dependían de un agente ejecutor inexistente  
- Eliminadas para mantener estabilidad  

---

## 🟢 FASE COMPLETADA

### 🟢 FASE 15 — Empaquetado Final
**Estado:** COMPLETA  
- PyInstaller funcional  
- `NOVA.exe` generado  
- Modelo incluido en `_internal/models`  
- Ejecución confirmada desde `dist/NOVA`  

---

## 🔴 FASE PENDIENTE (NUEVA)

### 🔴 FASE 16 — AGENTE EJECUTOR LOCAL
**Estado:** NO IMPLEMENTADA  

#### Descripción
Programa externo, separado de NOVA, encargado de ejecutar acciones reales en el sistema.

#### Responsabilidades
- Crear y modificar archivos  
- Ejecutar comandos  
- Usar programas instalados (VS Code, Python, etc.)  
- Compilar software  
- Generar instaladores  

#### Reglas
- El agente NO decide  
- NOVA solo envía instrucciones  
- Permisos limitados  
- Prohibido tocar Windows crítico (disco, registro, drivers)  

---

## 🧱 ARQUITECTURA FINAL REAL

