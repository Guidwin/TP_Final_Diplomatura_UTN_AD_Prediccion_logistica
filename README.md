# Evaluación de desempeño del sistema de logística de entrega (delivery logistic)– Proyecto Final Integrador


Este repositorio contiene el código y los recursos para el Proyecto Final Integrador del Diplomado en Ciencia de Datos y Análisis Avanzado. El objetivo es Predicción del tiempo de entrega de paquetes de distintos pesos y tamaños usando Machine learning, siguiendo la metodología CRISP‑DM.

## Contenido

Grupo_16_TP_Final Git hub.ipynb`: ejecutado en googlecolab con todo el análisis: carga de datos, ingeniería de variables, modelado (Bayesian Ridge -modelo benchmark- ,Regresión Lineal, SVR, LGBM, DNN), evaluación de métricas y explicación de variables mediante valores SHAP.
- `data/`: Carpeta donde deben colocarse el archivo `Delivery_Logistics.csv` descargados de Kaggle (ver instrucciones más abajo).
- `README.md`: Este archivo, que describe el proyecto, requisitos y cómo ejecutar el notebook.

## Requisitos

- Python 3.11 o superior.
- Librerías de Python: `pandas`, `numpy`, `scikit‑learn`, `matplotlib`. Opcionalmente, `shap` y `xgboost` si se desea experimentar con métodos adicionales de interpretabilidad o modelos más avanzados.

## Instalación

1. Clona o descarga este repositorio.
2. Crea un entorno virtual (opcional pero recomendado):

   ```bash
   python -m venv env
   source env/bin/activate


3. Instala las dependencias necesarias:

   ```bash
   pip install pandas numpy scikit-learn matplotlib
   # Si deseas usar la librería SHAP y XGBoost:
   pip install shap xgboost
   ```

## Descarga de Datos

Debes descargar el archivo `Delivery_Logistics.csv  provenientes de Kaggle y colocarlos en la carpeta donde se ejecutará el código. 
## Ejecución del Notebook
https://www.kaggle.com/datasets/muhammadahmaddaar/delivery-logistics-dataset-india-multi-partner(Kaggle).

1. Abre el notebook `Grupo_16_TP_Final Git hub.ipynb` con Jupyter Notebook o googlecolab:
  
2. Ejecuta las celdas en orden. El notebook realiza los siguientes pasos:

   * Importación de librerías y configuración.
   * Carga del dataset.
   * Ingeniería de variables y limpieza de datos.
   * Definición de modelos (Regresión Lineal,SVR, LGBM, entre otros ), entrenamiento y evaluación de métrica seleccionada.
   * Comparación de modelos y selección del modelo final.
   * Cálculo de valores SHAP aproximados para interpretar la Regresión Lineal.
   * Visualización de la importancia de las variables y explicación de los valores SHAP.

3. Al finalizar, podrás observar las métricas de cada modelo y los gráficos de valores SHAP que identifican las variables más influyentes.
