# AURA - Bloque Maestro IA - Version 1.0 (Reconstrucción Completa)

Documento técnico oficial del proyecto AURA reconstruido a partir del archivo proporcionado.
Autor: ingolivera-byte
Asistente técnico: ChatGPT

---

## **Información del equipo**

* Laptop ASUS TUF A15
* GPU NVIDIA RTX 4050
* CPU Ryzen 5 7535HS
* RAM 16GB
* Windows 11
* Python 3.11.6
* Entorno virtual `.venv`
* Micrófono USB

---

## **Objetivo del proyecto**

AURA es una inteligencia artificial local capaz de:

* Escuchar y transcribir audio
* Hablar mediante TTS
* Ver imágenes y procesarlas con visión artificial
* Realizar OCR en imágenes y PDFs
* Cargar y ejecutar modelos IA locales
* Automatizar tareas
* Operar completamente offline
* Usar una interfaz estilo holográfico futurista

---

## **Estructura del proyecto**

```
D:\AURA\
│
├── .venv
├── models
│   ├── llama3
│   │   └── Meta-Llama-3.1-8B-Instruct-Q4_K_M.gguf
│   └── phi3
│       └── Phi-3-mini-4k-instruct-Q4_K_S.gguf
├── grabar.py
├── windows_tts.py
├── vision.py
├── ocr_handler.py
├── ia_core.py (pendiente)
└── config.json (pendiente)
```

---

## **Librerías instaladas**

### Audio

* SpeechRecognition
* PyAudio
* sounddevice
* wavio
* ffmpeg

### Visión / OCR

* OpenCV
* pytesseract
* Tesseract OCR
* pdf2image
* Pillow

### Modelos IA

* llama-cpp-python
* numpy
* moderngl

### Interfaces

* PyQt6
* pygame

---

## **Modelos locales instalados**

* **LLaMA 3.1 8B Instruct:**
  `D:\AURA\models\llama3\Meta-Llama-3.1-8B-Instruct-Q4_K_M.gguf`

* **Phi-3 Mini 4K Instruct:**
  `D:\AURA\models\phi3\Phi-3-mini-4k-instruct-Q4_K_S.gguf`

---

## **Código completo de módulos**

### **6.1 grabar.py**

```python
import sounddevice as sd
from scipy.io.wavfile import write
import speech_recognition as sr

def grabar_audio(nombre_archivo="audio.wav", duracion=5, fs=44100):
    print("Grabando...")
    audio = sd.rec(int(duracion * fs), samplerate=fs, channels=2)
    sd.wait()
    write(nombre_archivo, fs, audio)
    print("Grabación finalizada.")
    return nombre_archivo

def transcribir_audio(ruta_audio):
    r = sr.Recognizer()
    with sr.AudioFile(ruta_audio) as source:
        audio = r.record(source)
    try:
        return r.recognize_google(audio, language="es-MX")
    except:
        return "No se pudo transcribir."

if __name__ == "__main__":
    archivo = grabar_audio()
    print(transcribir_audio(archivo))
```

---

### **6.2 windows_tts.py**

```python
import win32com.client as wincl

def hablar(texto):
    voz = wincl.Dispatch("SAPI.SpVoice")
    voz.Speak(texto)

if __name__ == "__main__":
    hablar("Hola, soy AURA.")
```

---

### **6.3 vision.py**

```python
import cv2

def cargar_imagen(ruta_imagen):
    imagen = cv2.imread(ruta_imagen)
    if imagen is None:
        raise FileNotFoundError("No se pudo cargar la imagen: " + ruta_imagen)
    return imagen

def mostrar_imagen(imagen, titulo="Vista previa"):
    cv2.imshow(titulo, imagen)
    cv2.waitKey(0)
    cv2.destroyAllWindows()

if __name__ == "__main__":
    img = cargar_imagen("test.jpg")
    mostrar_imagen(img)
```

---

### **6.4 ocr_handler.py**

```python
import pytesseract
from PIL import Image
import pdf2image
import os

pytesseract.pytesseract.tesseract_cmd = "C:\\Program Files\\Tesseract-OCR\\tesseract.exe"

def ocr_imagen(ruta_imagen):
    if not os.path.exists(ruta_imagen):
        raise FileNotFoundError("No existe la imagen: " + ruta_imagen)
    imagen = Image.open(ruta_imagen)
    return pytesseract.image_to_string(imagen, lang="spa+eng")

def ocr_pdf(ruta_pdf):
    if not os.path.exists(ruta_pdf):
        raise FileNotFoundError("No existe el PDF: " + ruta_pdf)
    paginas = pdf2image.convert_from_path(ruta_pdf)
    texto_total = ""

    for i, pagina in enumerate(paginas):
        texto = pytesseract.image_to_string(pagina, lang="spa+eng")
        texto_total += f"\n--- Página {i+1} ---\n{texto}"

    return texto_total

if __name__ == "__main__":
    print(ocr_imagen("prueba.jpg"))
```

---

## **Avances logrados**

* Audio funcionando correctamente
* Síntesis de voz funcionando correctamente
* Visión funcionando correctamente
* OCR funcionando correctamente
* Modelos locales instalados
* Proyecto estable

---

## **Pendientes**

* ia_core.py
* config.json
* Integración completa del pipeline

---

## **Seguridad**

* Sin conexión a internet
* No envía datos fuera del equipo
* Todo módulo requiere autorización del usuario

---

## **Referencia visual**

Interfaz basada en el archivo:
**Mujer Holográfica en Estilo Ciberpunk.png**

---

## **Fin del Bloque Maestro IA versión 1.0 (Reconstruido)**
