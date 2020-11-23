# Juego de la sepiente mediante el uso de Algoritmos genéticos
Red neuronal entrenada usando un algoritmo genético que actúa como el cerebro de la serpiente.

La serpiente mira en 8 direcciones en busca de alimento, parte del cuerpo y el límite que actúa como la entrada 24 para la red neuronal.

<video src= "/samples/Prueba_30_generaciones.mp4">

## Primeros pasos
### Prerrequisitos
Para instalar las dependencias, ejecute en la terminal :
```
python3 -m pip install -r requirements.txt
```

### Estructura del proyecto
```
├── Arena.py            # clase que ayuda a establecer los límites y los parámetros de la arena
├── brain.py            # clase que se ocupa de la red neuronal
├── colors.py           # clase donde consta de colores utilizados en todo el proyecto
├── game.py             # deja que las serpientes salvadas se ejecuten 
├── samples
│   ├── Prueba_30_generaciones.mp4    
├── input.py            # parámetros para aplicar el algoritmo genético por su cuenta
├── README.md
├── requirements.txt    # dependencias requeridas de Python
├── saved
│   └── top_snakes.pickle   # lista guardada de objetos de la clase snake para cada generación
└── snake.py            # clase que maneja todas las propiedades de la serpiente
```
## Entrenamiento
Para entrenar la red neuronal usando el algoritmo genético, modifique los parámetros de acuerdo a sus necesidades dentro de 'input.py', luego ejecute el siguiente comando especificando la ruta para guardar el resultado optimizado como un archivo pickle (se almacena una lista , que contiene la mejor serpiente de cada generación):
```
python3 Genetic_algo.py --output saved/test.pickle 
```
## Jugando
Para ejecutar o probar las serpientes guardadas previamente, ejecute los siguientes comandos especificando la ruta al archivo guardado :
```
python3 game.py --input saved/test.pickle
```
### Saltarse pasos
Para omitir pasos, simplemente agregue el argumento -s o --steps a la llamada
```
python3 game.py --input saved/test.pickle --steps 50
```

# Integrantes:
CALDERÓN AGUIRRE SAMUEL ISAÍAS
CALVA VICENTE DARWIN ESTEBAN
NARVAEZ NIETO FRANK WILLIAMS
OJEDA COLÁN DIEGO VALENTÍN
PAREDES DEMERA ELVIS FABRICIO
RAMÓN RAMÓN RICARDO ALEXANDER
TORRES VELEPUCHA JASON DAMIAN
