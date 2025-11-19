# Ejercicio: Métricas de Clasificación

Este notebook demuestra cómo calcular y visualizar métricas de evaluación para un problema de clasificación.

## Descripción

El programa utiliza la biblioteca `scikit-learn` para realizar los siguientes pasos:

1.  **Carga de Datos:** Lee un archivo `metricas.csv` que contiene dos columnas: `Clases real` y `Clases predicha`.
2.  **Matriz de Confusión:** Calcula y muestra la matriz de confusión para evaluar la precisión del modelo de clasificación. La matriz compara las clases reales con las predichas.
3.  **Reporte de Clasificación:** Genera y muestra un reporte de clasificación que incluye métricas clave como:
    *   **Precisión (Precision):** La proporción de predicciones positivas que fueron correctas.
    *   **Recall (Sensibilidad):** La proporción de positivos reales que fueron identificados correctamente.
    *   **F1-Score:** La media armónica de la precisión y el recall.

Este ejercicio es fundamental para entender cómo evaluar el rendimiento de un modelo de clasificación más allá de la simple exactitud (accuracy).
