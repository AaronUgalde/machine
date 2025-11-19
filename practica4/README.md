# Práctica 4: Comparación de Regresión Polinomial

Este notebook explora la Regresión Polinomial utilizando `scikit-learn` y compara su rendimiento bajo diferentes condiciones, incluyendo el método de optimización (OLS vs. SGD), el grado del polinomio y el escalado de características.

## Contenido

El notebook se divide en dos programas principales que utilizan datasets distintos.

### Programa 1: Regresión Polinomial en `datos.csv`

Esta parte se enfoca en un dataset con una sola característica para visualizar y comparar fácilmente las curvas de regresión.

-   **Dataset:** `datos.csv`
-   **Modelos Evaluados:**
    1.  **Regresión Lineal y Polinomial (Grados 2 y 3) con Mínimos Cuadrados Ordinarios (OLS).**
    2.  **Regresión Lineal y Polinomial (Grados 2 y 3) con Descenso de Gradiente Estocástico (SGD).**
-   **Análisis:**
    *   Se entrena cada modelo y se evalúa su rendimiento en un conjunto de prueba.
    *   Se generan gráficas que muestran la curva de predicción de cada modelo sobre los datos de prueba.
    *   Se reportan el Error Cuadrático Medio (MSE) y el coeficiente de determinación (R²) para comparar la bondad de ajuste de cada modelo.

### Programa 2: Regresión Polinomial Multivariable y Escalado en `cal_housing.csv`

Esta sección aborda un problema más complejo con múltiples características y evalúa el impacto del preprocesamiento de datos.

-   **Dataset:** `cal_housing.csv` (un dataset multivariable).
-   **Modelos Evaluados:**
    1.  **Regresión Lineal (Grado 1) con OLS.**
    2.  **Regresión Polinomial (Grados 2 y 3) con OLS.**
-   **Técnicas de Escalado:**
    *   Para los modelos polinomiales, se compara el rendimiento en tres escenarios:
        1.  Sin escalado de características.
        2.  Con **StandardScaler** (estandarización).
        3.  Con **RobustScaler** (robusto a outliers).
-   **Análisis:**
    *   Se presenta un resumen comparativo del MSE and R² para cada configuración, permitiendo analizar cómo el grado del polinomio y el método de escalado afectan el rendimiento del modelo en un dataset multivariable.

Este ejercicio es clave para entender cómo la complejidad del modelo (grado del polinomio) y el preprocesamiento de los datos (escalado) son factores determinantes en el rendimiento de los modelos de regresión.
