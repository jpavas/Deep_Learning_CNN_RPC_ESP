# DL-CNN-RPC
En este repositorio se encuenta todo el contenido asociado a la entrega del proyecto  **U3 (redes convolucionales)**, perteneciente al curso de posgrado Fundamentos de Deep Learning de la Universidad de Antioquia.

En el proyecto se utiliza el dataset Retail Product Checkout dataset (RPC), para aplicar estrategias de resolución como: Transfer learning, Featuring Learning, Arquitectura de red CNN; tareas de aprendizaje como: Classification, Image Segmentation y Occlussion; y métricas de evaluación como: cálculo y gráficos de accuracy y loss, matrices de confusión y muestras aletorias de imágenes con las etiquetas originales y sus predicciones. 

A continuación se detalla el contenido de cada notebook:

## U3.1 – Inicial
  
**Descarga y caracterización inicial del conjunto de datos:** Antes de explorar el contenido de este proyecto, es necesario **ejecutar completamente** este notebook.

### Contenido
1. Información general de la base de datos
2. Procesamiento inicial de imágenes
3. Descarga y descompresión del dataset ajustado
4. Decodificación del archivo .json para train
5. Traducción de nombres de los productos
6. Muestra de las imágenes del dataset

## U3.2.1 - Modelo CNN
	
**Creación y entrenamiento de una CNN (Preliminar):** A lo largo de esta sección, se realiza el ejercicio de crear una Red Neuronal Convolucional y llevar a cabo su entrenamiento con el conjunto de datos de Train. La idea es entrenar esta red para clasificar imágenes de acuerdo a las 17 super categorías del dataset RPC. Cabe destacar que, en este notebook, no se realizó validación cruzada para pérdida ni para precisión.

### Contenido
1. Importación de librerías y cargue del dataset RPC
2. Creación del Modelo CNN
3. Entrenamiento del modelo

## U3.2.2 - Modelo CNN - Transfer Learning Inception V3

**Transferencia de aprendizaje de InceptionV3 para el dataset RPC:** Se realiza Transfer Learning con el modelo InceptionV3, el cual fue pre-entrenado con el Dataset  Imagenet, para realizar tareas de clasificación con las 17 super categorías del dataset  Retail Product Checkout Dataset (RPC). En el proceso, la idea es utilizar InceptionV3 como extractor de características para facilitar la tarea de clasificación. El notebook tiene dos etapas:  Entrenamiento sin modificación de los pesos de InceptionV3 y  Fine-Tuning de algunas de las capas.

### Contenido
1. Actividades preliminares
2. Carga del modelo InceptionV3
3. Entrenamiento del modelo sin modificar los pesos de InceptionV3
4. Fine - Tuning en InceptionV3

## U3.2.3 - Modelo CNN con Validación

**Entrenamiento del modelo creado en U3.2.1 con validación usando GPU en Google Colaboratory:** Partiendo de las tareas realizadas en U3.2.1, donde se creó un modelo preliminar y se entrenó sin realizar validación, y de U3.2.2, donde se implementó Transfer Learning con InceptionV3 y se obtuvo un modelo con overfitting pese a los esfuerzos; se decidió volver a entrenar el modelo creado en U3.2.1, realizando validación y utilizando la GPU de Google Colaboratory (este notebook fue ejecutado en Colab para realizar el entrenamiento).

### Contenido
1. Importación de librerías y cargue del dataset RPC
2. Creación del modelo CNN
3. Entrenamiento del modelo CNN con validación en Colab

## U3.3 – Clasificación

**Clasificación con diferentes modelos CNN:** Se validarán diferentes arquitecturas de modelos CNN para clasificar imágenes del dataset Retail Product Checkout Dataset (RPC). Se pretende clasificar las 17 super categorías de dicho dataset y evaluar la precisión de las predicciones realizadas por los modelos respecto a las super categorías originales.

### Contenido
1. Importación de librerías y cargue del dataset RPC
2. Definición de las funciones para mostrar los resultados
3. Clasificación con el modelo CNN Test (U3.2.1)
4. Clasificación con el modelo Transfer Learning InceptionV3 (U3.2.2)
5. Clasificación con el modelo CNN Test con Validación (U3.2.3)

## U3.4 - Segmentacion - Feature Learning

**Segmentación utilizando aprendizaje de características (Feature Learning):** Se utilizará la segmentación semántica de imágenes del modelo Deep Lab para segmentar objetos del dataset RPC. Específicamente, se validará con objetos de la super categoría drink de RPC, los cuales serán tratados como objetos de la clase bottle en el modelo Deep Lab.

### Contenido
1. Importación de librerías y cargue del dataset RPC de test
2. Definición modelo Deep Lab
3. Validación Deep Lab con muestras del dataset

## U3.5 – Oclusión

**Oclusión utilizando la CNN entrenada con los datos del Dataset RPC:** Se realiza oclusión para tres imágenes, utilizando las 17 supercategorías del Dataset RPC. Para esto, se utilizará la red que fue creada y entrenada en el notebook "U3.3.3 - Modelo CNN con validación".

### Contenido
1. Tareas preliminares
    1.1 Importación de librerías y cargue del dataset RPC de test
    1.2 Cargue del modelo
    1.3 Creación de funciones
2. Oclusión de imágenes

### Contenido
1. Tareas preliminares
    - Importación de librerías y cargue del dataset RPC de test
    - Cargue del modelo
    - Creación de funciones
2. Oclusión de imágenes


