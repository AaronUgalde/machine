# Práctica: Descenso de Gradiente Interactivo

Este notebook proporciona una implementación interactiva de un algoritmo de descenso de gradiente para regresión lineal.

## Descripción

A diferencia de una implementación estándar de Descenso de Gradiente en Lote (BGD) o Estocástico (SGD), este programa está diseñado como una herramienta de aprendizaje interactiva.

-   **Dataset:** `data.csv`
-   **Objetivo:** Ajustar un modelo de regresión lineal a un pequeño conjunto de datos.
-   **Proceso Interactivo:**
    1.  El programa divide los datos en conjuntos de entrenamiento y prueba.
    2.  En cada iteración del bucle de entrenamiento, el programa **solicita al usuario** que ingrese:
        *   El índice `j` de la muestra de entrenamiento que se utilizará para calcular el gradiente.
        *   El valor de `alpha` (tasa de aprendizaje) para esa iteración.
    3.  El gradiente se calcula utilizando solo la muestra `j` seleccionada, y los pesos del modelo se actualizan en consecuencia.
    4.  Después de cada actualización, el modelo se evalúa en el conjunto de prueba y se muestran los pesos actualizados, la predicción y el error.

Este enfoque permite al usuario experimentar directamente con el efecto de seleccionar diferentes muestras y tasas de aprendizaje, observando su impacto inmediato en los pesos del modelo y el error de predicción. Es una demostración práctica de un único paso de actualización en un proceso de descenso de gradiente.
