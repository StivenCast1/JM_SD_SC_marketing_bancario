# 📈 Proyecto de Ciencia de Datos - Predicción de Suscripción a Depósitos Bancarios

Este proyecto desarrolla un flujo completo de **Machine Learning** utilizando el dataset **Bank Marketing** del UCI Repository.  
El objetivo es **predecir si un cliente aceptará una suscripción a un depósito a plazo**, basado en características personales y de interacción comercial.

## 🎯 Objetivos

- Realizar **Análisis Exploratorio de Datos (EDA)** usando visualizaciones interactivas con **Plotly**.
- Preprocesar datos utilizando **Pipelines** y **ColumnTransformer** (`scikit-learn`).
- Aplicar técnicas de:
  - Imputación de valores
  - Escalamiento
  - **OneHot Encoding**
  - **Label Encoding**
  - Reducción opcional de dimensionalidad (PCA)
- Entrenar y comparar al menos **2 modelos de Machine Learning**.
- Versionar el proyecto en **GitHub**.

- Carga de los datos directamente desde **Drive**.

## 🧱 Estructura del Proyecto

JM_SD_SC_MARKETING_BANCARIO
│
├─ datos/
│   └─ # Datos originales en drive (si se descargan localmente)
│
├─ notebooks/
│   └─ 01_descarga_datos.ipynb          Lectura inicial de los datos
│   └─ 02_exploracion_datos.ipynb       Exploración y ajuste de los datos
│   └─ 03_automl_flaml.ipynb            Comparativo de modelos (exploración modelos)
│   └─ 04_entrenamiento_modelo.ipynb    Entrenamiento, selección y guardado de Modelo lightgbm 
│
├
│
│
├─ requirements.txt
└─ README.md

## 🛠️ Instalación y Configuración

### 1) Crear entorno virtual
python -m venv .venv

Activar:
- Windows: .venv\Scripts\activate
- Linux/Mac: source .venv/bin/activate

### 2) Instalar dependencias
pip install -r requirements.txt

## 📥 Carga de Datos

### ✅ Opción 1: Archivo Local
Se lee el archivo de la siguiente ruta de Drive:
https://drive.google.com/file/d/1sfd6TnOHhrCq0I1TusC9HoRwgTtXohFr/view?usp=drive_link

## 🔍 EDA
Abrir notebooks/02_exploracion_datos.ipynb para análisis visual.

## 🧩 Entrenamiento
Notebooks/04_entrenamiento_modelo.ipynb



## 🧠 Nota Importante
Se elimina la variable `duration` para evitar fuga de información.

## 🚀 Subir a GitHub
git add .
git commit -m "Proyecto Bank Marketing"
git push origin main

## 👨‍💻 Autor
Sergio Durán, Jhonatan Mosquera, Stiven Castrillon
2025.
