# Predicción de default financiero usando métodos de aprendizaje automático
Los notebooks contenidos en este repositorio trabajan en la competición de Kaggle [Give Me Some Credit](https://www.kaggle.com/competitions/GiveMeSomeCredit) para proponer un modelo de machine learning que permite predecir la variable de salida para el conjunto de datos proveído. A nivel de negocio esto se interpreta como la capacidad para predecir si un usuario entrara en mora por más de 90 días.

## Estructura de Notebooks
### Preprocessing
En este notebook se realiza tareas de pre procesamiento en los datos con el fin de generar un dataset optimo para 
integrar en el modelo de machine learning. Algunas tareas como limpieza, eliminación de variables, detección de atípicos, 
renombrado de variables, entre otros, pueden verse en este notebook. 

El archivo resultante es el csv [Preprocessed](data/Preprocessed.csv) en la carpeta data del repositorio. 

### Model_Implementation_Train
Notebook donde se códifica la implementación del modelo y posterior entrenamiento.

El archivo resultante es el export del modelo seleccionado para ejecutar la validación.

### Model_Validation
En este notebook se hace la validación del modelo seleccionado con el dataset de validación proveído. También se realiza
un análisis de los resultados y conclusiones finales.



## Cómo ejecutar
El notebook fue ejecutado en el entorno jupyter. Se deben tener todas las librerías correspondientes para poder ejecutar los scripts.

Para la dependencia de XgBoost puede ejecutar este comando en la shell de conde. Previamente se debió seleccionar el ambiente virtual de trabajo.

`` 
conda install -c conda-forge py-xgboost
``

En la carpeta donde se ejecuto el notebook debe haber una carpeta hija llamada `GiveMeSomeCredit` que contenga la base de datos `cs-training.csv`.
