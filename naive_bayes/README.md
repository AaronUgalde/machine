# Implementación de Naive Bayes para Clasificación de Texto

Este notebook presenta una implementación desde cero (from scratch) del clasificador Naive Bayes para una tarea de clasificación de texto simple.

## Descripción

El objetivo es clasificar oraciones como positivas (`+`) or negativas (`-`). El algoritmo se implementa sin depender de las bibliotecas de alto nivel como `scikit-learn` para el modelo en sí.

El proceso es el siguiente:

1.  **Carga de Datos:** Se lee un conjunto de datos simple desde `Book1.csv`, que contiene oraciones y sus etiquetas de clase.
2.  **Cálculo de Probabilidades Previas (Prior):** Se calcula la probabilidad de cada clase (positiva y negativa) basándose en su frecuencia en el conjunto de entrenamiento.
3.  **Cálculo de Probabilidades Condicionales:**
    *   Se tokenizan las oraciones en palabras individuales.
    *   Para cada palabra, se calcula su probabilidad condicional dado una clase (ej. P(palabra | clase = +)).
    *   Se aplica el **suavizado de Laplace (Laplace Smoothing)** con un `alpha=1` para evitar probabilidades de cero para palabras que no han aparecido en una clase particular durante el entrenamiento.
4.  **Clasificación (Predicción):**
    *   Para una nueva oración, se calcula la probabilidad posterior (posterior probability) para cada clase posible.
    *   Esto se hace multiplicando la probabilidad previa de la clase por las probabilidades condicionales de todas las palabras en la oración.
    *   La clase con la probabilidad posterior más alta es la predicción final. Se utilizan logaritmos para evitar problemas de underflow numérico con probabilidades muy pequeñas.

Este ejercicio ilustra los mecanismos internos del algoritmo Naive Bayes y su aplicación en el procesamiento de lenguaje natural.
