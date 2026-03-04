# 📊 Predicción de Cancelación de Clientes (Churn Analysis) - TelecomX

![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange.svg)
![Pandas](https://img.shields.io/badge/Library-Pandas-brightgreen.svg)

Este proyecto desarrolla un modelo predictivo capaz de identificar qué clientes de una empresa de telecomunicaciones tienen mayor probabilidad de cancelar sus servicios. El objetivo es permitir que la empresa tome acciones proactivas de retención.

## 🎯 Objetivos del Proyecto
* **Preprocesamiento:** Limpieza, codificación de variables categóricas y normalización de datos.
* **Análisis Estadístico:** Selección de variables mediante pruebas de correlación y Chi-cuadrado.
* **Modelado:** Entrenamiento y comparativa de modelos de Clasificación (Regresión Logística y Random Forest).
* **Evaluación:** Análisis de rendimiento mediante matrices de confusión, reporte de métricas (F1-Score, Recall) y Curva ROC.
* **Insights:** Identificación de los factores críticos que influyen en la fuga de clientes.

## 🗂️ Estructura del Notebook
1. **Análisis Exploratorio (EDA):** Visualización de distribuciones y detección de valores nulos.
2. **Selección de Características:** Uso de pruebas estadísticas para identificar predictores clave como el tipo de contrato y servicios de seguridad.
3. **Pipeline de Machine Learning:**
   * Escalado de variables numéricas con `StandardScaler`.
   * Manejo de variables categóricas con `One-Hot Encoding`.
4. **Evaluación de Modelos:** Comparativa detallada entre modelos lineales y basados en árboles.

## 📈 Resultados Clave
* **Modelo Ganador:** Random Forest (debido a su capacidad para manejar relaciones no lineales).
* **Métrica Principal:** Se priorizó el **Recall** para minimizar los falsos negativos (clientes que se van y no fueron detectados).
* **Factor Crítico:** El tipo de contrato **Month-to-month** es el predictor más fuerte de cancelación.


## 💡 Recomendaciones Estratégicas
* **Migración de Contratos:** Incentivar el paso de contratos mensuales a anuales.
* **Fidelización Temprana:** Los clientes con menos de 10 meses de antigüedad requieren programas de acompañamiento intensivos.
* **Servicios de Valor:** Promover `TechSupport` y `OnlineSecurity`, ya que actúan como factores de retención.

## 🛠️ Tecnologías Utilizadas
* **Lenguaje:** Python
* **Librerías:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn.
* **Entorno:** Google Colab

---
Desarrollado como parte del desafío de modelado predictivo para TelecomX.
