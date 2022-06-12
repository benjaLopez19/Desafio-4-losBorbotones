# Desafio-4-losBorbotones
 Q-learning&DeepQ-learning
 
El código consiste en un jupyter notebook, que puede ser ejecutados usando python y algún editor de código como Visual Studio Code.

Mountain car
Este problema consta de llevar un carro por una pendiente hasta la meta. 
El espacio de acciones consta de 3 valores: acelerar hacia la izquierda, no acelerar y acelerar a la derecha. Mientras que el espacio de observación cuenta con 2 valores: posición de carro en el eje X, donde este puede ir entre -1,2 y 0.6; y velocidad, donde esta puede variar entre -0.07 y 0.07. 
El éxito se consigue al llegar al punto máximo, la bandera, por cada momento o timestep que este pase si alcanzarla, se le asignará un -1 a su puntuación. 
Un episodio terminará si se cumplen dos opciones: que el carro alcance la bandera o que hayan pasado 200 timesteps. Regresando el puntaje obtenido del episodio.
Los algoritmos a utilizar son Q-learning y Deep Q-learning.

Algoritmos
Por un lado Q-learning trabaja sobre una "Tabla Q" del tamaño del espacio de búsqueda del problema, para que luego el algoritmo de Q-learning se encarga de obtener las recompensas de las acciones que tome el agente sobre el ambiente, de manera que se tenga un aprendizaje sobre lo que se debe hacer en distintas situaciones. La tabla Q se rellena usando el algoritmo de bellman, de forma que los valores de recompensa no se cambien fijamente en la tabla Q sino que se ponderen de acuerdo a los resultados obtenidos en los episodios completados.
Por otro lado el Deep Q-learning opera de forma similar al Q-learning, solo que en vez de tener una tabla Q a rellenar para saber sobre el espacio de búsqueda, se tienen redes neuronales. Esto último se basa en que rara vez se podrá explorar el espacio de búsqueda completo (dado el tamaño que algunos ejemplos pueden tomar), por lo que rellenar una tabla con todos los casos (o si quiera intentar llegar a todos los casos) no se hace posible, así que el uso de redes neuronales para reemplazar la tabala Q soluciona este problema. Las redes se encargan de rescibir las recompensas del agente sobre el ambiente y pueden aprender para hacer predicciones sobre nuevos casos vistos.

Link del video: https://www.youtube.com/watch?v=aygmOdLKOnM
