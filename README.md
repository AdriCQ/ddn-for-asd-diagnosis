# Clasificación de Pacientes con TEA mediante Redes Neuronales Profundas (DNN)

Este repositorio contiene la implementación de un modelo de red neuronal profunda (DNN) para la clasificación de pacientes con Trastorno del Espectro Autista (TEA) y sujetos neurotípicos (TC). El modelo utiliza características extraídas de las matrices de conectividad funcional, calculadas a partir de series temporales promedio de regiones de interés (ROIs) definidas por diversos atlas cerebrales.

---

## Descripción General

El objetivo de este proyecto es desarrollar un sistema asistido por computadora para el diagnóstico de TEA basado en datos de conectividad funcional cerebral obtenidos de imágenes de resonancia magnética funcional en estado de reposo (rs-fMRI). Las principales etapas incluyen:

1. *Preprocesamiento de datos*: 
   - Generación de matrices de conectividad funcional utilizando métodos como correlación de Pearson y parametrización en espacio tangente.
   - Vectorización de matrices para obtener características representativas de cada sujeto.

2. *Entrenamiento del modelo DNN*: 
   - Diseño y ajuste de un modelo de red neuronal profunda para clasificación binaria.
   - Optimización de hiperparámetros mediante herramientas como Keras Tuner.

3. *Evaluación del modelo*:
   - Validación mediante cross-validation estratificada con datos divididos por grupos.
   - Comparación de resultados con diferentes pipelines de preprocesamiento y atlas cerebrales.