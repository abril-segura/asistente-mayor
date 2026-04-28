# Asistente Virtual para Adultos Mayores

Aplicación de escritorio interactiva diseñada con un enfoque profundo en la accesibilidad y la experiencia de usuario (UX) para personas de la tercera edad. El sistema combina una interfaz gráfica intuitiva con inteligencia artificial, síntesis de voz y visión computacional para asistir en el día a día.

## Características Principales

* **Asistente Conversacional (IA):** Integración con Google Gemini para mantener conversaciones dignas y maduras, brindando acompañamiento psicológico.
* **Gestor de Medicamentos:** Registro de tratamientos con cálculo automático de próximas tomas y alertas visuales/sonoras.
* **Visión Computacional (OCR):** Capacidad de leer cajas de medicamentos utilizando la cámara web y extraer el nombre y la dosis automáticamente.
* **Accesibilidad Total:** * Interfaz de Alto Contraste para usuarios con visión reducida.
  * Ajuste dinámico de tamaño de fuente.
  * Navegación controlada por voz y dictado inteligente con filtrado de datos (RegEx).
  * Síntesis de voz neuronal (Edge TTS) para lectura de pantalla.

## Requisitos Previos e Instalación

Para ejecutar este proyecto, es necesario tener instalado **Python 3.x** y el motor de reconocimiento óptico de caracteres **Tesseract OCR**.

### 1. Configurar Tesseract OCR
El sistema utiliza Pytesseract para leer las cajas de medicinas, Para que funcione correctamente en Windows:
    1. Descargar el instalador de Tesseract OCR para Windows
    2. Instalarlo en la ruta por defecto (C:\Program Files\Tesseract-OCR\tesseract.exe). De lo contraio, si desea instalarlo en otra ruta, deberá modificar la variable dentro pytesseract.pyteresseact.tesseract_cmd en el código fuente.

### 2. Instalar dependencias de Python
Abre tu terminal en la carpeta del proyecto y ejecuta el siguiente comando para instalar las librerías necesarias:
```bash
pip install -r requirements.txt
```

#### Ejecutar la aplicación
Una vez instaladas las dependencias y Tesseract, simplemente se ejecuta el archivo principal desde la terminal:
```bash
python asistente_mayor.py
```