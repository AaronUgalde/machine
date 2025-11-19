# Regresión Lineal con Mínimos Cuadrados Ordinarios (OLS)

Este notebook implementa el algoritmo de Regresión Lineal por Mínimos Cuadrados Ordinarios (Ordinary Least Squares - OLS) desde cero para un conjunto de datos simple.

## Descripción

El objetivo es encontrar la línea que mejor se ajusta a un conjunto de puntos de datos. El algoritmo no utiliza bibliotecas de machine learning como `scikit-learn` para el cálculo de los coeficientes.

El proceso es el siguiente:

1.  **Definición de Datos:** Se crea un pequeño conjunto de datos de entrenamiento y otro de prueba.
2.  **Cálculo de Coeficientes (OLS):**
    *   Se calculan los coeficientes de la recta de regresión (`y = b0 + b1*x`) utilizando las fórmulas matemáticas de OLS.
    *   `b1` (la pendiente) y `b0` (el intercepto) se derivan a partir de las sumatorias de `x`, `y`, `xy` y `x^2`.
3.  **Predicción:** Una vez calculados los coeficientes `b0` y `b1`, se utilizan para predecir los valores de `y` para el conjunto de datos de prueba.
4.  **Cálculo del Error:** Se calcula y muestra el error absoluto entre los valores reales de `y` y los valores predichos para cada punto del conjunto de prueba, demostrando la precisión del modelo.

Este ejercicio sirve para comprender los fundamentos matemáticos detrás del método de Mínimos Cuadrados Ordinarios en la regresión lineal.
