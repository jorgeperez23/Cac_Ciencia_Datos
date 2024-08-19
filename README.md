# Cac_Ciencia_Datos
## Trabajo Final Codo a Codo Fundamentos de Ciencia de Datos

# Codo a Codo Curso de Especializacion en Fundamentos de la Ciencia de datos
Este curso está dirigido a quienes posean conocimientos básicos de planillas de cálculo, SQL en base de datos y programación. Podrán incorporar los
conocimientos necesarios para preparar los datos que permitirán plantear,
analizar, predecir y solucionar problemas para asistir a las empresas en la toma de decisiones frente a los desafíos organizacionales.
Conocerán los conceptos, procesos y tecnologías involucrados. Aprenderán a utilizar herramientas de Python y sus librerías, y de Machine learning que
permitirán realizar un análisis predictivo.

## Objetivos del proyecto

Predecir la cantidad de crímenes por categorías según el conjunto de datos.
Contemplar:

    La limpieza y adecuación de los datos, incluída su separación para entrenamiento y testeo.(*)
    La transformación adecuada de los datos.
    Selección de variables de entrada (Features) y su justificación.
    Seleccion de características para el modelo, los hiperparámetros (si fuesen necesarios) y su justificación.
    Selección del modelo y las métricas para su evaluación y su justificación.
    Los métodos gráficos para la discusión del modelo.
    Argumentar brevemente aplicaciones para la predicción realizada.

### Introducción
  
  Preparación de Datos: Técnicas para limpiar y organizar datos.
  
  Análisis de Datos: Métodos para analizar y visualizar datos.
  
  Predicción y Modelado: Uso de algoritmos de machine learning para predicciones

## Herramientas y Tecnologías

Python: Lenguaje de programación principal.

Librerías de Python: Pandas, NumPy, Matplotlib, Scikit-learn.

## Ciclo de Vida de un Proyecto de Ciencia de Datos:

  Recolección de Datos: Fuentes y métodos.
  
  Limpieza y Preparación: Técnicas de preprocesamiento.
  
  Análisis Exploratorio: Identificación de patrones y tendencias.
  
  Modelado Predictivo: Construcción y evaluación de modelos.

### Descripción del Notebook

#### Sección 1: Importar librerías en Python
                Se instalan las librerías necesarias para realizar los distintos procedimientos (ejemplo: numpy, pandas, matplotlib, seaborn, sklearn)
#### Sección 2: Montado de Google Drive y Carga de Datos
                Se realizan dos métodos para montar la carpeta de Google Drive donde esta alojados los datos.
                Luego se cargan los datos a un dataframe de pandas con el nombre de df_delitos_22
#### Sección 3: EDA Análisis Exploratorios de Datos
                Se busca información del dataset como (los nombres de las columnas, tipo de datos, no-null)
                Se limpian los datos, quitando faltantes y columnas que no vamos a utilizar con el comando drop
                Se crean dos gráficas con seaborn 1) barplot para contar los delitos por comunas y 2) boxplot para verificar los outliers
#### Sección 4: Feature y Target
                Se aplica la técnica de OneHotEncoder para convertir las variables categóricas de la columna Tipo en varias columnas con los diferentes tipos de delitos (Amenazas,Homicidios, Hurto,Lesiones, Robo,Vialidad)
                Para poder utilizar esas columnas en nuestros modelos lineales
#### Sección 5: Modelo de Regresión Logístico
                Dividimos los datos en Entrenamiento / Test para poder justamente entrenar nuestro modelo
                Creamos nuestro modelo de Regresión Logística utilizando la librería scikit learn 
                Mostramos los valor que el modelo nos arroja, basados en la bondad de ajuste
                Luego visualizamos los valores importante de la predicción del modelo (ejemplo MSE, MAE, M, RSS, RMSE)
                Se crea un gráfico con matplotlib
                Creamos un modelo statsmodels y visualizamos los valores
                
## Conclusiones
Nuestro modelo de Regresión Logística, no muestra la curva de una función sigmoide, por ende no se está cumpliendo las características del modelo. Las variables tienen una alta correlación.

Tenemos un RMSE: 0.63 y una Bondad de ajuste: 0.59

Que son bajas para considerar este modelo viable.

## Recomendaciones

Por este motivo no podemos recomendar la utilización de este modelo de Regresión Logística, para futuros análisis del dataset del delito en CABA.

Hasta que realicemos las pruebas suficientes para poder mejorar dicho modelo en el futuro
    
