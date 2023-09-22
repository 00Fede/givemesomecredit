# Monografía presentada para optar al título de Especialista en Analítica y Ciencia de Datos

Este repositorio contiene los notebooks generados en el trabajo de monografía titulada "Predicción de default financiero usando métodos de aprendizaje automático", presentada por los estudiantes Federico Ocampo Ortiz y Andrés Felipe Orrego Quintero como requisito para obtener el título de Especialista en Analítica y Ciencia de Datos. El trabajo fue desarrollado bajo la asesoría de la Ph.D. Maria Bernarda Salazar Sánchez.

## Resumen
El objetivo de este Desarrollar un modelo para predecir si una persona entrará en mora por 90 días tal que permita a entidades bancarias definir el riesgo financiero asociado a una solicitud de crédito. Los notebooks contenidos en este repositorio trabajan en la competición de Kaggle [Give Me Some Credit](https://www.kaggle.com/competitions/GiveMeSomeCredit).


## Estructura de Notebooks
### Preprocessing
En este notebook se realizan las tareas de preprocesamiento de los datos, con el fin de generar un dataset óptimo para 
integrar en el modelo de machine learning. Algunas tareas como limpieza, eliminación de variables, detección de atípicos, 
renombrado de variables, entre otros, pueden verse en este notebook. 

El archivo resultante es el csv [Preprocessed](data/Preprocessed.csv) alojado en la carpeta data del repositorio. 

### Model_Implementation_Train
En este notebook  se códifica la implementación del modelo y su posterior entrenamiento, así como la selección de los mejores hiperparámetros.

El archivo resultante es el export del modelo seleccionado para ejecutar la validación.

### Model_Validation
En este notebook se hace la validación del modelo seleccionado con el dataset de validación, incluyendo además el análisis de los resultados y conclusiones finales.

## Cómo ejecutar
El notebook fue ejecutado en el entorno jupyter. Se deben tener todas las librerías correspondientes para poder ejecutar los scripts.

Para la dependencia de XgBoost puede ejecutar este comando en la shell de conde. Previamente se debió seleccionar el ambiente virtual de trabajo.

`` 
conda install -c conda-forge py-xgboost
``

En la carpeta donde se ejecutó el notebook debe haber una carpeta hija llamada `GiveMeSomeCredit` que contenga la base de datos `cs-training.csv`.
