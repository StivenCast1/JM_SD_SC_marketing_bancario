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
- Construir una **app interactiva** con **Streamlit**.
- Versionar el proyecto en **GitHub**.
- (Opcional) Cargar los datos directamente desde **OneDrive**.

## 🧱 Estructura del Proyecto

bank-marketing-ml/
│
├─ datos/
│   └─                        # Datos originales (si se descargan localmente)
│
├─ notebooks/
│   └─ Descarga_datos.ipynb           # Exploración de datos con Plotly
│   └─ Exploracion_datos.ipynb           # Exploración de datos con Plotly
│
├─ src/
│   ├─ data.py                # Carga de datos (local u OneDrive)
│   ├─ models.py              # Pipelines y ColumnTransformer
│   ├─ train.py               # Entrenamiento y evaluación de modelos
│   └─ app.py                 # Aplicación Streamlit
│
├─ reports/
│   └─ figures/               # Gráficos generados en el EDA
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
Coloca el archivo bank-full.csv en:
data/raw/bank-full.csv

Y cárgalo:
df = pd.read_csv("data/raw/bank-full.csv", sep=';')

### 🌐 Opción 2: Desde OneDrive (Enlace Público)
df = pd.read_excel("https://1drv.ms/xxxxx?download=1")

## 🔍 EDA
Abrir notebooks/01_eda.ipynb para análisis visual.

## 🧩 Entrenamiento
python src/train.py

## 🎛️ Aplicación Streamlit
streamlit run src/app.py

## 🧠 Nota Importante
Se elimina la variable `duration` para evitar fuga de información.

## 🚀 Subir a GitHub
git add .
git commit -m "Proyecto Bank Marketing"
git push origin main

## 👨‍💻 Autor
Sergio Durán, Jhonatan Mosquera, Stiven Castrillon
2025.
