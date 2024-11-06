
# Proyecto de Análisis de Churn de Clientes Bancarios

Este proyecto realiza un análisis sobre la probabilidad de pérdida de clientes (churn) en un banco, entrenando varios modelos de machine learning para predecir el churn y seleccionando el modelo con mejor rendimiento.

## Descripción del Proyecto

El conjunto de datos contiene información sobre clientes de un banco. En este análisis, se examinan las características de los datos, se manejan datos faltantes y se entrenan diferentes modelos para predecir la probabilidad de que un cliente abandone el banco.

## Estructura del Análisis

1. **Introducción y Preparación de los Datos**
   - Se cargan los datos del archivo `Churn.csv`.
   - Se identifican y manejan valores faltantes, especialmente en la columna "Tenure".

2. **Análisis Exploratorio de Datos (EDA)**
   - Se examinan las características principales de los datos, tales como distribución de clientes y tiempo de relación con el banco.
   - Se crean visualizaciones con `plotly` para ilustrar las características demográficas y de comportamiento de los clientes.

3. **Entrenamiento de Modelos de Machine Learning**
   - Se implementan modelos de clasificación como `RandomForestClassifier`, `LogisticRegression` y `DecisionTreeClassifier`.
   - Se utiliza `GridSearchCV` para ajustar los hiperparámetros y seleccionar el mejor modelo.
   - Se aplican técnicas de sobremuestreo (`SMOTE`) para balancear las clases.

4. **Evaluación de Modelos**
   - Los modelos se evalúan utilizando métricas como el **F1 Score**, **AUC-ROC**, **Recall** y **Precision**.
   - Se selecciona el modelo con mejor rendimiento para predecir el churn de clientes bancarios.

5. **Conclusiones**
   - El análisis concluye con una discusión sobre los modelos evaluados y su efectividad en la predicción de churn.

## Requisitos

- **Python 3.7+**
- Librerías: `pandas`, `numpy`, `scikit-learn`, `imblearn`, `plotly`

## Cómo Ejecutar el Proyecto

1. Clona el repositorio.
2. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```
3. Ejecuta el notebook para reproducir el análisis y las visualizaciones.
