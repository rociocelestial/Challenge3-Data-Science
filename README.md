# Challenge3-Data-Science
Telecom X - parte 2 : Predicción de Cancelación (Churn)

## 🎯 Misión

La es  misión es desarrollar modelos predictivos capaces de prever qué clientes tienen mayor probabilidad de cancelar sus servicios.

La empresa quiere anticiparse al problema de la cancelación, y te corresponde a ti construir un pipeline robusto para esta etapa inicial de modelado.


## 🧠 Objetivos del Desafío

* Preparar los datos para el modelado (tratamiento, codificación, normalización).

* Realizar análisis de correlación y selección de variables.

* Entrenar dos o más modelos de clasificación.

* Evaluar el rendimiento de los modelos con métricas.

* Interpretar los resultados, incluyendo la importancia de las variables.

* Crear una conclusión estratégica señalando los principales factores que influyen en la cancelación.

# 📡 Telecom X: Predicción de Churn (Parte 2)

Este proyecto forma parte de un análisis avanzado de ciencia de datos enfocado en la retención de clientes para la empresa de telecomunicaciones **Telecom X**. El objetivo principal es construir un modelo predictivo capaz de determinar la probabilidad de que un cliente cancele su servicio (**Churn**) basándose en variables clave del negocio. 📉

## 🛠️ Tecnologías Utilizadas
Para este análisis y modelado, se emplearon las siguientes herramientas del ecosistema de Data Science:

* **Lenguaje:** ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
* **Manipulación de Datos:** ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
* **Visualización:** ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![Seaborn](https://img.shields.io/badge/Seaborn-blue?style=for-the-badge&logo=Seaborn&logoColor=white)
* **Machine Learning:** ![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
* **Entorno:** ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white) ![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)

---

## 1. 🎯 Propósito del Proyecto
El abandono de clientes es uno de los desafíos más costosos en el sector de las telecomunicaciones. Este análisis busca:
* **Predecir el Churn:** Identificar a los usuarios con mayor riesgo de salida antes de que suceda. ⚠️
* **Identificar Variables Clave:** Entender qué factores (tipo de contrato, cargos mensuales, servicios adicionales) influyen directamente en la decisión del cliente. 🔍
* **Acción Proactiva:** Proporcionar una base sólida para que el equipo de marketing diseñe estrategias de fidelización personalizadas. 💡

---

## 2. 📂 Estructura del Proyecto
```
TelecomX_Churn_Analysis/
├── 📁 data/
│   ├── raw_telecom_data.csv       # Datos originales
│   └── processed_telecom.csv      # Datos limpios y codificados para el modelo
├── 📁 notebooks/
│   └── TelecomX_Parte2_Model.ipynb # Cuaderno principal con el análisis y modelado
├── 📁 reports/
│   └── 🖼️ figures/                # Gráficos e insights exportados (Matplotlib/Seaborn)
├── 📄 requirements.txt            # Librerías necesarias para ejecutar el proyecto
└── 📄 README.md                   # Documentación del proyecto


```


---
## 3. ⚙️ Preparación de los Datos y Modelado
El proceso de preparación fue fundamental para garantizar la calidad de las predicciones:

**📊 Clasificación de Variables**
* **Variables Categóricas:** Género, tipo de contrato, método de pago y servicios (DSL/Fibra). 🗂️

* **Variables Numéricas:** Tenencia (meses), cargos mensuales y cargos totales. 🔢

### 🛠️ Ingeniería de Características (Preprocessing)
* **Codificación:** Transformación de variables cualitativas a formatos numéricos procesables. 💻

* **Normalización:** Escalado de datos numéricos para asegurar que la Regresión Logística converja sin sesgos por magnitud. ⚖️

* **División de Datos:** Separación estricta de 80% para entrenamiento y 20% para prueba (train/test split). ✂️

### 🧠 Algoritmo Seleccionado: Regresión Logística
Se seleccionó la **Regresión Logística** como el modelo final. A diferencia de otros algoritmos complejos, permite una interpretación clara de los coeficientes, facilitando al negocio entender exactamente qué variables pesan más en la decisión de abandono de un cliente. 📈

---
## 4. 📈 Insights y Visualizaciones (EDA)
Durante el Análisis Exploratorio de Datos (EDA), se obtuvieron los siguientes hallazgos:

* **Factor de Permanencia:** Los clientes en sus primeros 6 meses presentan la mayor vulnerabilidad de abandono. ⏳

* **Tipo de Contrato:** Los contratos mes a mes tienen un Churn significativamente más alto que los anuales. 📅

* **Cargos Mensuales:** Se observó una correlación directa: a mayores cargos mensuales, aumenta la probabilidad de cancelación. 💰

---

## 5. 📊 Evaluación del Modelo
El desempeño final del modelo de Regresión Logística basado en el reporte de clasificación es:

| Métrica | Clase "No" (Fieles) | Clase "Yes" (Churn) | General (Accuracy) |
| :--- | :---: | :---: | :---: |
| **Precision** | 0.91 | 0.51 | **0.74** ✅ |
| **Recall** | 0.73 | **0.79** 🔔 | |
| **F1-Score** | 0.81 | 0.62 | |

---

**Nota sobre el desempeño:** Se destaca el Recall de 0.79 para la clase "Yes". Esto indica que el modelo es capaz de capturar al 79% de los clientes que realmente abandonarán, permitiendo a Telecom X tomar medidas preventivas sobre la gran mayoría de los casos de riesgo.

---

## 🚀 Instrucciones de Ejecución

### 📋 Requisitos Previos
Asegúrate de tener instaladas las siguientes librerías:

Bash

pip install pandas matplotlib seaborn scikit-learn

### 💻 Pasos para Ejecutar

Clona el repositorio y verifica que el archivo processed_telecom.csv esté en la carpeta data/. 📥

Abre el cuaderno TelecomX_Parte2_Model.ipynb en VS Code o Google Colab. 📒

Ejecuta las celdas secuencialmente para entrenar el modelo y visualizar la Matriz de Confusión. ▶️






