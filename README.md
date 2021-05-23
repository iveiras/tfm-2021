# Predicción de cáncer de mama mediante el uso de CNNs en mamografías
Código asociado al Trabajo Fin de Máster de Iago Veiras Lens para el Máster de Ciencia de Datos de la Universitat Oberta de Catalunya (UOC), presentado en junio de 2021.

## Descripción del trabajo
Implementación de una arquitectura de dos ramas DenseNet que toman como input las dos vistas (CC y MLO) de las mamografías, dando como predicción la etiqueta en Bi-Rads del caso clínico asociado.

## Librerías necesarias
Para poder ejecutar todos los notebooks del repositorio, es necesario disponer de las siguientes librerías:
* pandas
* glob2
* os
* skimage
* cv2
* matplotlib
* imblearn
* albumentations
* random
* tensorflow
* sklearn
* pickle5 (si se ejecuta desde entorno Google Colab)

## Detalle de los notebooks
A continuación se incluye una breve descripción de los notebooks del repositorio:
*  __Preprocesamiento_Imágenes__: preparación del dataset INbreast, aplicando técnicas de limpieza, homogeneización y balanceo.
*  __Particionamiento_dataset__: particionado del dataset en dos conjuntos que mantengan la proporción de etiquetas.
*  __Entrenamiento_DenseNet_1Rama__: entrenamiento de una arquitectura basada en DenseNet para una de las vistas de las mamografías (CC/MLO).
*  __Entrenamiento_DenseNet_2Ramas__: entrenamiento de una arquitectura de dos ramas DenseNet que toma como input las dos vistas (CC y MLO).
*  __Optimización_DenseNet_1Rama__: búsqueda de hiperparámetros para la arquitectura basada en DenseNet para una de las vistas de las mamografías (CC/MLO).
*  __Optimización_DenseNet_2Ramas__: búsqueda de hiperparámetros para la arquitectura de dos ramas DenseNet que toma como input las dos vistas (CC y MLO).
