# Age Prediction from Images

✅ Project Description
A supermarket chain aims to evaluate whether it is possible to estimate customers' age using computer vision, in order to support age verification in alcohol sales.
This project focuses on predicting a person's age from facial images using deep learning.
The target metric was to achieve a Mean Absolute Error (MAE) lower than 8 on the test set.

✅ Objective
Build and evaluate a regression model that can:
- Predict age from facial images
- Generalize across different age ranges
- Meet the defined error threshold

✅ Methodology

Data Preparation
- Load labels (labels.csv)
- Use data generators to handle images efficiently
- Normalize pixel values
- Split data into training and validation sets

Exploratory Data Analysis
- Check for missing values (none found)
- Analyze age distribution (imbalanced toward ages 20–40)
- Identify potential impact on model performance

✅ Modeling
- Use ResNet50 with pretrained weights from ImageNet (transfer learning)
- Adapt the model for a regression task
- Apply data augmentation during training
- Loss function: MSE
- Evaluation metric: MAE
- Early Stopping to prevent overfitting

✅ Technologies Used
- Python
- Pandas
- NumPy
- TensorFlow / Keras
- Matplotlib

✅ Results
The model achieved an MAE lower than 8, meeting the project objective.
Better performance was observed in age ranges with higher representation in the dataset, while performance decreased for underrepresented age groups.
Predicción de Edad a partir de Imágenes

✅ Descripción del proyecto
Una cadena de supermercados busca evaluar si es posible estimar la edad de los clientes mediante visión por computadora, con el objetivo de apoyar la validación en la venta de alcohol.
Este proyecto consiste en predecir la edad de una persona a partir de imágenes faciales utilizando deep learning.
La métrica objetivo fue lograr un Error Absoluto Medio (MAE) menor a 8 en el conjunto de prueba.

✅ Objetivo
Construir y evaluar un modelo de regresión que permita:
- Predecir la edad a partir de imágenes faciales.
- Generalizar correctamente en distintos rangos de edad.
- Cumplir con el umbral de error definido.

✅ Metodología

# Preparación de datos:
- Carga de etiquetas (labels.csv)
- Uso de generadores para procesar imágenes sin saturar memoria
- Normalización de píxeles
- División en entrenamiento y validación

Análisis exploratorio
- Revisión de valores nulos (sin incidencias)
- Distribución de edades (desbalance hacia 20–40 años)
- Identificación de posibles impactos en el modelo

✅ Modelado
- Uso de ResNet50 con pesos preentrenados en ImageNet (transfer learning)
- Adaptación a problema de regresión
- Data augmentation en entrenamiento
- Función de pérdida: MSE
- Métrica de evaluación: MAE
- Early Stopping para controlar sobreajuste

✅ Tecnologías utilizadas
- Python
- Pandas
- NumPy
- TensorFlow / Keras
- Matplotlib

✅ Resultados
El modelo logró un MAE menor a 8, cumpliendo con el objetivo del proyecto.
Se observó mejor desempeño en rangos de edad con mayor representación en los datos y mayor dificultad en edades extremas.
