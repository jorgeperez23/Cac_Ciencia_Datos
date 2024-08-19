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

### Introduccion
  
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

### Descripcion del Notebook

#### Seccion 1: Importar librerias en Python
                Se instalan las librerias necesarias para realizar los distintos procedimientos (ejemplo: numpy, pandas, matplotlib, seaborn, sklearn)
#### Seccion 2: Montado de Google Drive y Carga de Datos
                Se realizan dos metodos para montar la carpeta de Google Drive donde esta alojados los datos.
                Luego se cargan los datos a un dataframe de pandas con el nombre de df_delitos_22
#### Seccion 3: EDA Analisis Exploratorios de Datos
                Se busca informacion del dataset como (los nombres de las columnas, tipo de datos, no-null)
                Se limpian los datos, quitando faltantes y columnas que no vamos a utilizar con el comando drop
                Se crean don graficas con seaborn 1) barplot para contar los delitos por comunas y 2) boxplot para verificar los outliers
