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


# 📡 Proyecto TelecomX - Parte 2 : Predicción de Churn con Machine Learning

¡Bienvenido! Este proyecto aplica ciencia de datos para resolver uno de los problemas más críticos en las telecomunicaciones: la **fuga de clientes** (Churn). 

## 🎯 Objetivo
Identificar proactivamente a los clientes con mayor riesgo de abandonar la compañía para implementar estrategias de retención efectivas y salvar la rentabilidad del negocio.

---

## 🛠️ Herramientas Utilizadas
* **Lenguaje:** Python 🐍
* **Entorno:** Google Colab 🚀
* **Librerías:** Pandas, Matplotlib, Seaborn, Scikit-learn.
* **Modelos:** Regresión Logística, Árbol de Decisión y Random Forest.

---

## 📈 Lo que se hizo (Paso a Paso)

1. **Análisis de Datos (EDA):** Exploramos una base de +7,000 clientes, detectando que el 26% se había fugado. 🔍
2. **Preprocesamiento:** Limpiamos los datos y convertimos variables categóricas para que los modelos pudieran entenderlas. ⚙️
3. **Entrenamiento de Modelos:** Probamos 3 algoritmos distintos para encontrar el más preciso. 🤖
4. **Evaluación:** Usamos matrices de confusión y métricas de **Recall** para elegir el modelo ganador. ✅

---

## 🏆 El Ganador: Regresión Logística
Elegimos este modelo porque logró un **Recall de 0.79**. 
> **¿Qué significa esto?** Que logramos detectar a **8 de cada 10 clientes** antes de que se vayan. ¡Es el modelo que más dinero le ahorra a la empresa! 💰

---

## 💡 Hallazgos y Estrategia
El análisis reveló que los clientes se van principalmente por:
* 📑 **Contratos mes a mes:** Son muy inestables.
* 💸 **Facturas altas:** Existe un límite crítico de **$93.67**.
* 🌐 **Servicio de Fibra:** Presenta puntos de fricción que debemos mejorar.

### 🚀 Plan de Acción:
* **Migración:** Incentivar el paso a contratos anuales con meses de regalo. 🎁
* **Escuadrón de Retención:** Contactar a quienes superen los $93 de factura antes de que se quejen. 📞
* **Plan de Bienvenida:** Premiar la lealtad de los clientes nuevos al cumplir 6 meses. 🌟

---




*¡Gracias por revisar mi proyecto! Si tienes alguna duda o sugerencia, no dudes en contactarme.* 😊
