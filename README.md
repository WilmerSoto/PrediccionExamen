# PrediccionExamen
En este repositorio se encuentra el codigo relacionado al trabajo de "Predicción del rendimiento de estudiantes en un examen de matematicas, lectura y escritura".

# Instrucciones
Luego de realizar el cargue de los archivos, se puede optar por cargar los datos mediante regresion o clasificacion. Se puede optar por usar scaling o no en los datos, de igual forma en las metricas de evaluacion este no afecto de manera considerable.

Luego, se puede optar por que variables se quieren predecir. Existen tres opciones:
* math vs reading/writing.
* writing vs math/reading. 
* reading vs math/writing.

En el trabajo relacionado a este dataset se escogio al final la ultima opcion. <br>

Igualmente, en cada opcion se anoto los resultados de cada modelo. El primer valor es el R2 de Train, el segundo es el R2 de Test y el ultimo es el MAE de Test.<br>

Para clasificacion solo se tiene para predecir reading/writing con math. Pero en este reading y writing estan en y separadas.

<br>Dataset: https://www.kaggle.com/datasets/spscientist/students-performance-in-exams
