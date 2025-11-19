# Práctica 3: Regresión Lineal con Descenso de Gradiente en Lote (BGD)

Esta carpeta contiene dos implementaciones desde cero (from scratch) del algoritmo de **Descenso de Gradiente en Lote (Batch Gradient Descent - BGD)** para regresión lineal.

## Contenido

1.  **`bgd_monovariable.ipynb`**: Implementación de BGD para regresión lineal con **una sola variable**.
2.  **`bgd_multivariable.ipynb`**: Implementación de BGD para regresión lineal con **múltiples variables**.

Ambos notebooks se desarrollan sin utilizar las funciones de regresión de alto nivel de `scikit-learn` para ilustrar los mecanismos internos del algoritmo.

### 1. BGD Monovariable

-   **Dataset:** `casas.csv`
-   **Objetivo:** Predecir el precio de una casa basándose en el tamaño del terreno.
-   **Proceso:**
    1.  Divide el dataset en conjuntos de entrenamiento (70%) y prueba (30%).
    2.  Implementa el algoritmo BGD para ajustar iterativamente un único peso (pendiente de la recta).
    3.  En cada iteración, calcula el gradiente sobre todo el conjunto de entrenamiento para actualizar el peso.
    4.  Visualiza la convergencia del modelo, mostrando cómo la línea de predicción se ajusta a los datos de prueba y cómo el error disminuye a lo largo de las iteraciones.

### 2. BGD Multivariable

-   **Dataset:** `Dataset_multivariable.csv`
-   **Objetivo:** Predecir un valor `y` a partir de cinco características de entrada (`x1` a `x5`).
-   **Proceso:**
    1.  Divide el dataset en conjuntos de entrenamiento (70%) y prueba (30%).
    2.  Implementa el algoritmo BGD para ajustar simultáneamente un vector de pesos (uno para cada característica).
    3.  Al igual que en el caso monovariable, el gradiente se calcula utilizando todo el lote de datos de entrenamiento en cada paso.
    4.  El notebook muestra el proceso de actualización de los pesos y la evaluación del modelo en el conjunto de prueba.

Estos ejercicios permiten comprender cómo el Descenso de Gradiente en Lote optimiza los parámetros de un modelo de regresión, tanto en el caso simple de una variable como en el más general de múltiples variables.
