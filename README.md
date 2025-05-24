# MLT-Regresion


Objetivo del proyecto:

Aplicar técnicas de aprendizaje automático tradicional de regresión para predecir el precio de un automóvil según sus propiedades, aplicando un análisis exploratorio de datos (EDA) completo, para identificar patrones relevantes en el conjunto de datos, realizar selección de características mediante la ganancia de información mutua, comparar el desempeño de múltiples algoritmos de regresión mediante la librería LazyPredict, seleccionar el modelo óptimo en función de métricas de error como el Mean Squared Error (MSE) o Mean Absolute Error (MAE), y registrar de manera sistemática los resultados, métricas y artefactos generados durante el proceso utilizando la plataforma de seguimiento de experimentos MLflow.

=======================================================================

Descripción del dataset:

Dataset: Car Features and MSRP

Fuente: Kaggle ----> https://www.kaggle.com/datasets/CooperUnion/cardataset/data

El archivo se carga directamente desde un archivo .zip de la nube

  Acerca del conjunto de datos

Conjunto de datos de automóviles con características que incluyen marca, modelo, año, motor y otras propiedades del automóvil utilizadas para predecir su precio.

=======================================================================

Decisiones tomadas en el modelado:

Se usaron las características con menor cardinalidad y con un mínimo de información mutua del 0.3:  'Make', 'Year', 'Engine Fuel Type', 'Engine HP', 'Engine Cylinders', 'Vehicle Style', 'highway MPG', 'city mpg', 'Popularity'

Usando Lazypredict se seleccionó el modelo ExtraTreeRegressor por su desempeño y tiempo de ejecución.
El código final fue adaptado a la ejecución en github usando deepseek, originalmente fue hecho en google colab y mostrando las métricas en mlflow con ngrok

=======================================================================

Resultados y métricas principales:
mse: 74819855.19912094

mae: 3191.198386132693

r2_score: 0.9686101705137609
