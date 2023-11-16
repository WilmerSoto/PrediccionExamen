<a href="https://colab.research.google.com/github/WilmerSoto/PrediccionExamen/blob/main/Trabajo_final.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
# PrediccionExamen
En este repositorio se encuentra el codigo y dataset relacionado al trabajo de "Predicción del rendimiento de estudiantes en un examen de matematicas, lectura y escritura".

# Contenidos dataset
El dataset 'StudentsPerfomance.csv' se agarro originalmente de <a href="https://www.kaggle.com/datasets/spscientist/students-performance-in-exams">Kaggle</a>, este contiene un total de 8 columnas. 
- Genero
- Etnia
- Nivel educacion padres
- Tipo merienda
- Curso preparacion
- Nota lectura
- Nota matematicas
- Nota escritura
  
De las cuales se usaran como variables de entrada desde 'Genero' hasta 'Nota lectura', y se predecira 'Nota matematicas' y 'Nota escritura'.

# Instrucciones
Este repositorio contiene el notebook y el dataset usado. Si se quiere ejecutar en colab solamente basta con presionar el boton 'Open in Colab' que se encuentra arriba y cargar el archivo 'StudentsPerformance.csv' que se encuentra en este mismo repo.

Si se desea ejecutar localmente, se descarga ambos archivos 'Trabajo_final.ipynb' y 'StudentsPerformance.csv' y se ejecutan de forma local en cualquier editor de codigo que soporte Jupyter Notebooks.

Primero, se importan las librerias a usar y luego se hace la carga de los datos. 

Luego de realizar el cargue de los archivos, se puede optar por cargar los datos mediante regresion o clasificacion. Se puede optar por usar scaling o no en los datos, de igual forma en las metricas de evaluacion este no afecto de manera considerable.

Luego, se puede optar por que variables se quieren predecir en regresion. Existen tres opciones:
* math vs reading/writing.
* writing vs math/reading. 
* reading vs math/writing.
  
Igualmente, en cada opcion se anoto los resultados de cada modelo. El primer valor es el R2 de Train, el segundo es el R2 de Test y el ultimo es el MAE de Test.<br>

En el trabajo relacionado a este dataset se escogio al final la ultima opcion. <br>

Para clasificacion solo se tiene para predecir reading/writing con math. Pero en este reading y writing estan en Y separadas.

Luego de que elijas si probar regresion o clasificacion, mas abajo en el codigo se encuentra divididos los modelos en dos secciones. 'Regresion' y 'Clasificacion', se expande esos bloques de codigo y se encuentran diversos modelos para cada uno y cada uno con su respectiva metrica de validacion.

Cada modelo ya viene con un param_grid definido para la optimizacion de hiperparametros con GridSearch, solo basta con cargar el param_grid y poner a ejecutar la busqueda de GridSearch. Luego de que GridSearch retorna un modelo, este se guarda en una variable y abajo de esto siempre esta una prueba con una metrica de validacion para conocer su precision y/o exactitud.
