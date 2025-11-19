# Práctica 1: Métodos de Validación

Este notebook es un ejercicio práctico que demuestra el uso de diferentes estrategias de validación y división de datos utilizando la biblioteca `scikit-learn`.

## Descripción

El objetivo es familiarizarse con las técnicas fundamentales para la creación de conjuntos de entrenamiento, prueba y validación, que son cruciales para evaluar el rendimiento de los modelos de aprendizaje automático de manera robusta.

Se exploran los siguientes métodos sobre el dataset `metodosDeValidacion.csv`:

1.  **División Simple (Train-Test Split):**
    *   Se utiliza `train_test_split()` para dividir el conjunto de datos en un 70% para entrenamiento y un 30% para pruebas, sin mezclar los datos.

2.  **Validación Cruzada (K-Fold):**
    *   Se implementa `KFold()` para dividir el conjunto de datos de entrenamiento en `k=6` pliegues (folds). En cada iteración, un pliegue se utiliza para validación y los `k-1` restantes para entrenamiento.

3.  **Leave-One-Out (LOO):**
    *   Se utiliza `LeaveOneOut()`, una forma extrema de validación cruzada donde `k` es igual al número de muestras. En cada paso, un solo dato se usa para la validación y el resto para el entrenamiento.

4.  **Bootstrap:**
    *   Se demuestra el uso de `resample()` para crear conjuntos de validación mediante la técnica de Bootstrap. Esto implica muestreo con reemplazo para generar múltiples conjuntos de entrenamiento del mismo tamaño que el original.

El notebook imprime los conjuntos generados por cada método, permitiendo una comprensión clara de cómo funciona cada técnica de validación.
