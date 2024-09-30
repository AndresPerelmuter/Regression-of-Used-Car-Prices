# Regression-of-Used-Car-Prices

# Descripción del Proyecto
Este repositorio contiene mi participación en la competencia Playground Series - Season 4, Episode 9 - Regression of Used Car Prices en Kaggle. El objetivo de la competencia es predecir el valor de la variable price. 

La competencia está orientada a incentivar la experimentación y la mejora en la implementación de técnicas de Machine Learning y Deep Learning. A continuación, se detallan los pasos clave, enfoques y técnicas que he utilizado para abordar este desafío.

https://www.kaggle.com/competitions/playground-series-s4e9/leaderboard#

# Pasos Principales

1 - Preprocesamiento de Datos
Se implementaron diversas técnicas para limpiar y preparar los datos para el modelado. Algunos pasos incluyen:

- Visualización de Valores Faltantes: Se realizó un análisis para identificar la presencia de valores nulos en el dataset.

- Tratamiento de Valores Nulos: Para manejar los valores faltantes, se aplicó la moda (el valor más frecuente) en las columnas correspondientes, asegurando que no se introdujeran sesgos en el modelo.

- Codificación de Variables Categóricas: Se utilizó Label Encoder para convertir variables categóricas en valores numéricos, lo que permitió su inclusión en el modelo de manera eficiente.


2 - Análisis Exploratorio de Datos (EDA): Se ha realizado un análisis detallado del conjunto de datos para identificar patrones, anomalías y relaciones entre las variables. Esto incluye:

- Visualización de distribuciones.
- Evaluación de correlaciones.
- Análisis de valores faltantes (si aplicable).

3 - Modelado: Se ha probado una variedad de modelos de Machine Learning, centrándose principalmente en:

- LightGBM: Un algoritmo de Gradient Boosting optimizado para velocidad y eficiencia en grandes datasets.
- CatBoost: Especialmente diseñado para trabajar con características categóricas, proporcionando resultados robustos.
- XGBoost: Conocido por su rendimiento en competiciones de Machine Learning, este modelo es altamente eficiente y eficaz.

4 - Optimización de Hiperparámetros: Se utilizó **Optuna**, una biblioteca de optimización de hiperparámetros, para mejorar el rendimiento del modelo. Optuna permite la búsqueda automática de los mejores hiperparámetros a través de técnicas como el optimizador de TPE (Tree-structured Parzen Estimator). Esto se traduce en una búsqueda más eficiente y efectiva en comparación con métodos de búsqueda manual o en cuadrícula, ayudando a encontrar configuraciones óptimas que maximizan el rendimiento del modelo.

5 - Evaluación del Modelo: Los modelos fueron evaluados utilizando **RMSE (Root Mean Squared Error)**, que proporciona una medida de la diferencia promedio entre las predicciones del modelo y los valores reales. Esta métrica es especialmente útil en problemas de regresión, ya que penaliza más los errores grandes, ofreciendo una visión clara del rendimiento del modelo.

