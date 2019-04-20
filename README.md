# DL-CNN-RPC
En este repositorio se encuenta todo el contenido asociado a la entrega del proyecto  **U3 (redes convolucionales)**, perteneciente al curso de posgrado Fundamentos de Deep Learning de la Universidad de Antioquia.

En el proyecto se utiliza el dataset Retail Product Checkout dataset (RPC), para aplicar estrategias de resolución como: Transfer learning, Featuring Learning, Arquitectura de red CNN; tareas de aprendizaje como: Classification, Image Segmentation y Occlussion; y métricas de evaluación como: cálculo y gráficos de accuracy y loss, matrices de confusión y muestras aletorias de imágenes con las etiquetas originales y sus predicciones. 

A continuación se detalla el contenido de cada notebook:

## U3.1 – Inicial
  
  Descarga y caracterización inicial del conjunto de datos. Antes de explorar el contenido de este proyecto, es necesario **ejecutar completamente** este notebook.
  
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
