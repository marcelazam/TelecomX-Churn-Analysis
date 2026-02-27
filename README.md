# 📊 TelecomX — Churn Analysis & Prediction

## 📌 Descripción
Proyecto de análisis y predicción de cancelación de clientes (Churn) para una empresa de telecomunicaciones.

El objetivo es identificar los factores que influyen en la pérdida de clientes y construir modelos de Machine Learning que permitan predecir qué usuarios tienen mayor riesgo de cancelar el servicio, apoyando la toma de decisiones de negocio y estrategias de retención.

---

## 🎯 Objetivos
- Limpiar y preparar los datos
- Analizar el comportamiento del churn
- Explorar relaciones entre variables
- Dividir datos en entrenamiento y prueba
- Entrenar modelos de Machine Learning
- Evaluar métricas de desempeño
- Identificar variables más importantes
- Generar conclusiones accionables para el negocio

---

## 🗂️ Dataset
El dataset incluye información de clientes como:
- Datos demográficos
- Tipo de contrato
- Servicios contratados
- Cargos mensuales y totales
- Variable objetivo: **Churn (cancelación)**

---

## ⚙️ Proceso del proyecto

### 🔹 1. Preparación de datos
- Limpieza de valores nulos y espacios vacíos
- Conversión de variables numéricas
- Eliminación de columnas irrelevantes
- Creación de variable binaria `Churn_bin`

### 🔹 2. Análisis Exploratorio (EDA)
Se realizaron:
- Distribución de churn
- Boxplots de tenure y cargos vs churn
- Matriz de correlación
- Análisis dirigido de variables clave

**Hallazgos principales:**
- Menor tenure → mayor probabilidad de cancelación
- El gasto mensual influye, pero no es determinante por sí solo

### 🔹 3. Separación de datos
- 70% entrenamiento
- 30% prueba
- División estratificada para mantener proporción de churn

### 🔹 4. Modelos entrenados

#### Logistic Regression
- Datos normalizados
- Modelo interpretable
- Buen accuracy general

#### Random Forest
- Sin normalización
- Captura relaciones no lineales
- Mejor equilibrio entre precision y recall

### 🔹 5. Evaluación
Métricas utilizadas:
- Accuracy
- Precision
- Recall
- ROC-AUC

El modelo **Random Forest** presentó un desempeño ligeramente superior para detectar clientes con riesgo de churn.

### 🔹 6. Importancia de variables
Variables más relevantes:
- tenure
- Charges.Monthly
- Charges.Total

El tiempo de permanencia fue el factor más determinante.

---

## 📈 Resultados
- Los clientes nuevos cancelan con mayor frecuencia
- tenure es el predictor más fuerte
- Los modelos permiten anticipar cancelaciones con buen rendimiento

---

## 💡 Conclusiones
- Implementar estrategias de retención temprana
- Incentivar contratos de mayor duración
- Aplicar modelos predictivos para contactar clientes en riesgo
- Usar análisis de datos para decisiones comerciales más efectivas

---

## 🛠️ Tecnologías utilizadas
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

---

## ▶️ Cómo ejecutar
1. Abrir el notebook en Google Colab o Jupyter
2. Ejecutar **Entorno de ejecución → Reiniciar y ejecutar todo**
3. El análisis es completamente reproducible

---

## 👩‍💻 Autora
Marcela Zamora  
Data Science Student
