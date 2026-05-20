<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=120&section=header&animation=fadeIn" />
</div>

<h1 align="center">💇‍♀️ Detección y Modificación de Color de Cabello</h1>

<h3 align="center">🚀 Segmentación con YOLOv8 y Procesamiento de Imágenes</h3>

<p align="center">
  Proyecto de Computer Vision para la detección de cabello en imágenes de rostros y la posterior modificación de su color.<br>
  Implementado con Python, Ultralytics (YOLOv8) y OpenCV, abordando retos de segmentación de instancias y manipulación de espacios de color (HSV).
</p>

---

## 📋 **Descripción del Proyecto**

**Hair Color Detection** es un proyecto enfocado en la aplicación práctica de redes neuronales convolucionales de segmentación (YOLOv8-seg) para extraer con precisión la región del cabello en imágenes de alta resolución (dataset CelebA-HQ). El estudio incluye el procesamiento de máscaras binarias para aislar el cabello y la manipulación matemática de los canales Hue y Saturation para aplicar tintes virtuales fotorrealistas sin afectar el rostro o el fondo.

> ⚠️ **Estado del Proyecto:** Terminado
> Modelos entrenados, evaluados y pruebas de recoloreo satisfactorias.

---

## 🏗️ **Arquitectura Evaluada**

Se implementó un flujo completo de Deep Learning y Visión Clásica:
- **YOLOv8-seg (Nano):** Modelo de última generación de Ultralytics para segmentación de instancias. Destaca por su alta velocidad y precisión, ideal para inferencia rápida.
- **OpenCV (Procesamiento HSV):** Uso de máscaras como filtros bit-a-bit (`bitwise_and`) para el aislamiento de clases y la modificación selectiva del color sin alterar la luminosidad original de la imagen.

---

## 🔧 **Stack Tecnológico**

### **Lenguaje y Frameworks Core**
<div align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img width="8" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img width="8" />
  <img src="https://img.shields.io/badge/YOLOv8-00FFFF?style=for-the-badge&logo=yolo&logoColor=black" />
</div>

### **Procesamiento y Visualización de Datos**
<div align="center">
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" />
  <img width="8" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img width="8" />
  <img src="https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white" />
  <img width="8" />
  <img src="https://img.shields.io/badge/Pillow-3776AB?style=for-the-badge&logo=python&logoColor=white" />
</div>

### **Herramientas de Desarrollo**
<div align="center">
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white" />
  <img width="8" />
  <img src="https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" />
  <img width="8" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
</div>

---

## 🚀 **Estructura de Ejecución**

| Entorno | Archivo/Notebook | Objetivo Principal |
|-------|------------------|--------------------|
| **Local** | `notebook/hair_color_detection_local.ipynb` | Entrenamiento e inferencia en entorno local (Windows). |
| **Cloud (GPU)** | `notebook/hair_color_detection_colab.ipynb` | Entrenamiento optimizado en Google Colab, incluyendo integración directa con Google Drive. |

---

## 🏪 **Características Técnicas Implementadas**

### **🔍 Técnicas de Deep Learning & CV**
- Procesamiento automático del dataset CelebA-HQ y CelebAMask-HQ para extraer contornos y generar formato YOLO.
- Entrenamiento de segmentación instanciada (1 clase: Cabello).
- Transformación de la predicción probabilística multicanal a una **Máscara Binaria (0/255)** estricta.

### **🎨 Procesamiento de Imagen**
- Aislamiento matemático de píxeles empleando la máscara como un filtro (operaciones lógicas `bitwise`).
- Desplazamiento circular del espectro de color en el espacio **HSV** (canal *Hue*).
- Preservación de brillos y sombras originales (canal *Value*) para garantizar el fotorrealismo del tinte virtual.

---

👨💻 Desarrollador
<div align="center">
Santiago Arbelaez Contreras

Junior Full Stack Developer

Estudiante de Ingeniería de Sistemas – Universidad del Quindío

<br> <a href="https://github.com/santiagoarbelaezc"> <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /> </a> <img width="10" /> <a href="https://www.linkedin.com/in/santiago-arbelaez-contreras-9830b5290/"> <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /> </a> <img width="10" /> <a href="https://portfolio-santiagoa.web.app/portfolio"> <img src="https://img.shields.io/badge/Portfolio-6C63FF?style=for-the-badge&logo=sparkles&logoColor=white" /> </a></div>

<div align="center"> <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=90&section=footer&animation=fadeIn" /> </div>
