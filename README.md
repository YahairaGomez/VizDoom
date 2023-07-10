# VizDoom
VizDoom permite a los investigadores y desarrolladores utilizar el motor del juego Doom para entrenar y probar algoritmos de inteligencia artificial en entornos simulados. Proporciona una interfaz programática que permite a los agentes de IA interactuar con el juego, recibir información del entorno y tomar decisiones en función de esa información.

### Instalación 🔧
Para instalar y correr el proyecto descargue la carpeta la carpeta completa y ejecute el programa en el IDE Zinjai.

### Experimento 1 🔧 
<img src="https://github.com/YahairaGomez/VizDoom/blob/main/imagenes/experimento1.png">


### Experimento 2 🔧 
<img src="https://github.com/YahairaGomez/VizDoom/blob/main/imagenes/experimento2.png">


### Preguntas:
1. Como es el modelo del mundo utilizado: MDP, Modelo de premios y modelo Q-Learning.
El procesamiento de aprendizaje es similar al Deep Q-Learning introducido para Atari 2600. El problema se modela como un proceso de decisión de Markov y se utiliza Q-Learning para aprender la política. 

2. Qué tipo de política es usada.
La acción es seleccionada por una política ε-greedy con decadencia lineal ε.

3. Cómo se calculan y aproximan los valores Q.
La función Q se aproxima con una red neuronal convolucional. La red utilizada en el experimento consta de dos capas convolucionales con 32 filtros cuadrados, de 7 y 4 píxeles de ancho, respectivamente. A cada capa de convolución le sigue una capa de agrupación máxima con agrupación máxima de tamaño 2 y unidades lineales rectificadas para la activación. A continuación, hay una capa totalmente conectada con 800 unidades lineales rectificadas con fugas y una capa de salida con 8 unidades lineales correspondientes a los 8 combinaciones de las 3 opciones disponibles (izquierda, derecha y disparo).

4. Qué modelo de optimización se usa.
Se entrena con gradiente estocástica descendiente.

5. ¿Existe estrategia de repetición de experiencias?
Si existe.

### Análisis de ejecución, tiempo de proceso, uso de memoria, uso de CPU/GPU para los dos experimentos.  🔧

### Experimento 1 🔧 
<img src="https://github.com/YahairaGomez/VizDoom/blob/main/imagenes/resultadoCPU.png">


### Experimento 2 🔧 
<img src="https://github.com/YahairaGomez/VizDoom/blob/main/imagenes/resultadoCPU.png">

## Autores✒️

* **Yahaira Gomez** - *Documentación* - [YahairaGomez](https://github.com/YahairaGomez)
* **Christopher Yquira** - *Documentación* - [alexa1999](https://github.com/alexa1999)

## Expresiones de Gratitud 🎁

* Agradecimiento especial a YouTube y a la cafeína ☕
