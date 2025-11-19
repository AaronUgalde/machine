# Práctica: Clasificador Naive Bayes

Este notebook implementa y evalúa el clasificador Naive Bayes en dos datasets diferentes: `iris.csv` y `emails.csv`.

## Descripción

El programa realiza los siguientes pasos:

1.  **Carga de Datos:** Carga los datasets `iris.csv` y `emails.csv`.
2.  **Preprocesamiento:** Divide cada dataset en conjuntos de entrenamiento (70%) y prueba (30%).
3.  **Entrenamiento y Validación Cruzada:**
    *   Implementa dos variantes del clasificador Naive Bayes:
        *   **Gaussiano (Normal):** Adecuado para características continuas que siguen una distribución normal.
        *   **Multinomial:** Utilizado comúnmente para características discretas (como conteo de palabras).
    *   Utiliza validación cruzada (k-fold, con k=3) en el conjunto de entrenamiento para comparar el rendimiento de ambos modelos y seleccionar el mejor para cada dataset.
4.  **Evaluación Final:**
    *   Entrena el mejor modelo seleccionado en la etapa anterior con todo el conjunto de entrenamiento.
    *   Evalúa el rendimiento del modelo final en el conjunto de prueba, que no fue utilizado durante el entrenamiento.
5.  **Visualización de Resultados:**
    *   Muestra tablas comparativas con la precisión (accuracy) de cada pliegue de la validación cruzada.
    *   Para la evaluación final, genera:
        *   La matriz de confusión.
        *   Un reporte de clasificación completo (precisión, recall, f1-score).
        *   Una visualización gráfica de la matriz de confusión.

Este ejercicio permite comparar la aplicabilidad y el rendimiento de diferentes distribuciones de Naive Bayes en datasets con características distintas.
