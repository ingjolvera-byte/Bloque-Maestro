# 🧠 BLOQUE MAESTRO DE DESARROLLO DE AURA — Versión 0.4
## ✔ Estado técnico estable y verificado  
## 👤 Autor: ingolivera-byte  
## 🤖 Sistema Asistente: ChatGPT  

---

# 🧩 1. Información del Equipo
- **Laptop:** ASUS TUF A15  
- **GPU:** NVIDIA RTX 4050  
- **CPU:** AMD Ryzen 5 7535HS  
- **RAM:** 16 GB  
- **SO:** Windows 11  
- **Python:** 3.11.6  
- **Entorno:** `.venv` activo  
- **Micrófono:** USB operativo  

---

# 🧩 2. Objetivo del Proyecto
Construir una **IA local avanzada llamada AURA**, capaz de:

- Hablar y escuchar  
- Ver e interpretar imágenes  
- Leer PDFs y realizar OCR  
- Crear software y automatizar tareas  
- Operar completamente local  
- Tener una interfaz holográfica (según referencia visual)

---

# 🧩 3. Estructura Actual del Proyecto

```
D:\AURA\
│── .venv\
│── models\
│   ├── llama3\
│   │   └── Meta-Llama-3.1-8B-Instruct-Q4_K_M.gguf
│   └── phi3\
│       └── Phi-3-mini-4k-instruct-Q4_K_S.gguf
│
│── audio.wav
│── grabar.py
│── windows_tts.py
│── vision.py
│── (pendiente) ocr_handler.py
│── (pendiente) ia_core.py
│── (pendiente) config.json
```

---

# 🧩 4. Librerías Instaladas

### ✔ Audio
- SpeechRecognition  
- PyAudio  
- sounddevice  
- wavio  
- ffmpeg  

### ✔ Visión y OCR
- OpenCV  
- pytesseract  
- Tesseract OCR instalado  
- pdf2image  

### ✔ Interfaces
- PyQt6  
- pygame  

### ✔ Modelos IA
- llama-cpp-python  
- numpy  
- moderngl  

---

# 🧩 5. Modelos Disponibles Localmente

### ✔ Meta LLaMA 3.1 8B — Q4_K_M  
Ruta:  
```
D:\AURA\models\llama3\Meta-Llama-3.1-8B-Instruct-Q4_K_M.gguf
```

### ✔ Phi-3 Mini 4K Instruct — Q4_K_S  
Ruta:  
```
D:\AURA\models\phi3\Phi-3-mini-4k-instruct-Q4_K_S.gguf
```

---

# 🧩 6. Archivos Funcionales

## ✔ 6.1 grabar.py  
Código verificado. Graba audio y realiza transcripción.

## ✔ 6.2 windows_tts.py  
Código verificado. AURA ya puede generar voz.

## ✔ 6.3 vision.py (FUNCIONAL)
```python
import cv2

def cargar_imagen(ruta_imagen: str):
    """
    Carga una imagen desde una ruta específica.
    """
    imagen = cv2.imread(ruta_imagen)
    if imagen is None:
        raise FileNotFoundError(f"No se pudo cargar la imagen: {ruta_imagen}")
    return imagen

def mostrar_imagen(imagen, titulo: str = "Vista previa de la imagen"):
    """
    Muestra la imagen en una ventana.
    """
    cv2.imshow(titulo, imagen)
    cv2.waitKey(0)
    cv2.destroyAllWindows()

if __name__ == "__main__":
    ruta = "test.jpg"  # Cambiar por una imagen real para probar
    img = cargar_imagen(ruta)
    mostrar_imagen(img)
```

---

# 🧩 7. Avances Técnicos Logrados
- Audio funcionando (grabación + transcripción)  
- Voz funcionando (TTS Windows SAPI5)  
- Visión funcionando (OpenCV)  
- Modelos locales listos  
- OCR instalado  

---

# 🧩 8. Pendientes (Siguientes módulos)

### ⏳ 8.1 ocr_handler.py  
### ⏳ 8.2 ia_core.py  
### ⏳ 8.3 config.json  

---

# 🧩 9. Seguridad del Sistema
- Nada se ejecuta sin autorización  
- Sin internet salvo permiso explícito  
- Sin envío de datos externos  
- Protección estricta del sistema  

---

# 🧩 10. Referencia visual oficial de la Interfaz de AURA
**Imagen:** `Mujer Holográfica en Estilo Ciberpunk.png`  
*(Esta será la estética exacta de la interfaz cuando lleguemos a esa fase)*  

---

# 🟪 FIN DEL BLOQUE MAESTRO — Versión 0.4 (OFICIAL Y LIMPIA)
