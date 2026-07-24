Clasificación de Tumores Cerebrales mediante CNN y Optimización con Grid Search

Este repositorio contiene el desarrollo y la evaluación de modelos de Redes Neuronales Convolucionales (CNN) diseñados para la detección automatizada de tumores cerebrales a partir de imágenes de Resonancia Magnética (MRI). El enfoque principal es la optimización sistemática de hiperparámetros para garantizar el máximo rendimiento diagnóstico.

📋 Resumen del Proyecto

El proyecto implementa un pipeline de aprendizaje profundo que abarca desde el preprocesamiento de imágenes hasta la búsqueda exhaustiva de arquitecturas óptimas mediante Grid Search. Se evaluaron múltiples configuraciones de capas, filtros y funciones de activación, logrando identificar un modelo de alto rendimiento con una exactitud del 94.16%.

🛠️ Especificaciones Técnicas y Reproducibilidad

Para cumplir con los estándares de reproducibilidad exigidos en entornos científicos, se detallan los parámetros técnicos utilizados:
  
  ● Dataset: Brain Tumor Classification (MRI) de Kaggle. https://doi.org/10.34740/kaggle/dsv/2645886
  
  ● División de Datos: 80% entrenamiento, 10% validación y 10% prueba (Semilla aleatoria: 1337).  
  
  ● Entorno de Ejecución: Google Colab utilizando una GPU NVIDIA A100-SXM4-40GB. 
  
  ● Configuración de Entrenamiento:Batch Size: 32. 
  
  ● Épocas: 20 (máximo).  
  
  ● Early Stopping: Paciencia de 3 épocas monitoreando val_loss para prevenir el sobreajuste.  
  
  ● Semilla de Carga (Data Loader): 123. 
  

📊 Resultados del Modelo Óptimo

Tras el proceso de Grid Search, el modelo con mejor desempeño (ID: 20241123-070745) presentó las siguientes métricas:  

● MétricaValorExactitud (Accuracy): 94.16%

● AUC (Área bajo la curva ROC): 99.09%

● Pérdida (Loss): 16.38%

● Sensibilidad (Recall): 92.72%


🚀 Tecnologías

● Python 3.

● xTensorFlow / Keras

● Scikit-learn
