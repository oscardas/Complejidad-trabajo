# Complejidad-trabajo

Complejidad Algorítmica
Trabajo Parcial

Tema: Quoridor

Docente: Luis Martin Canaval Sanchez

Integrantes: 

-Flores Palermo, Oscar Daniel

-Cacha Panduro, Juben

-Thom Merino, Damian








Ciclo Académico: 2020-2





Índice
Introducción

Estado del Arte

Metodología






























Introducción:
En el siguiente informe se desarrollará el proyecto llamado quoridor, que consiste en desarrollar un juego donde participan 2 o 4 jugadores(bots o personas). 
La principal meta para los jugadores será la de llegar al otro lado del tablero mientras impiden que el rival avance poniendo muros frente al otro. Para la creación 
del juego se realizará el uso de diferentes algoritmos enfocados a la optimización y a la inteligencia artificial del bot.

Estado del Arte:
Desde la creación de las computadoras, se ha investigado mucho sobre las tareas que estas pueden realizar y así se llegó a la implementación de las inteligencias 
artificiales que hoy en día conocemos como tal. Sin embargo, detrás de cada una se encuentran una serie de algoritmos que hacen posible su funcionamiento y de las 
cuales se explicará en las siguientes líneas. Si nos enfocamos en el funcionamiento de algoritmos dentro de las IA, podemos usar a los juegos con ̈bots ̈ programados 
como ejemplo para entender mejor su uso. 

Primero, tenemos a un algoritmo llamado MINMAX, que define a las decisiones del jugador oponente como decisiones óptimas y tendrá que basarse en esta dificultad, por 
lo que si el jugador oponente es inexperto este perderá fácilmente. Luego, está el algoritmo "Primero el mejor" que se caracteriza por su búsqueda y elección de caminos, 
ya que este no escoge caminos en base a las interacciones sino las escoge en base a los caminos más óptimos. Por ejemplo en el popular juego "Pacman", donde los fantasmas 
buscan un camino corto para atrapar al jugador.

Por último, existen momentos en todo juego donde las decisiones a tomar son muy amplias y el estar probando todas sería un desperdicio de memoria y aquí entra el algoritmo 
"Poda alfa-beta", que mejora los límites colocados por el algoritmo MINMAX, ya que define a los límites dentro de un rango infinito para ambos extremos y solo se reducirá 
si es que un nodo tiende a ser menor, reduciendo así a menores búsquedas.

Metodología:
Cómo funciona el juego
El tablero de Quoridor consta de una cuadrícula de 9x9, y cada jugador controla una pieza, que debe comenzar desde un borde del tablero. Las piezas deben ubicarse en el 
centro de la fila y enfrentarse entre sí. Antes de comenzar, se divide los 20 bloques en partes iguales (si cada jugador juega en parejas, cada jugador tiene 10, y si cada 
jugador juega en parejas, hay 5). El bloque debe estar en la ranura entre cada casillero. Con su ancho, cada bloque cortará dos filas o dos columnas de caminos. No está 
permitido rodear completamente al oponente. En cada ronda, el jugador puede elegir mover su peón, el peón sólo puede avanzar una casilla por ronda y no puede moverse 
\en diagonal o colocar nuevas paredes, siempre y cuando no las use todas. Cuando dos peones se enfrentan (cara a cara), pueden saltar a otro, avanzar dos casillas 
excepcionalmente o evitarlo moviendo una casilla en diagonal hacia adelante.

como pensamos que funciona
El juego lo vemos que funciona con un jugador y un IA (bot) los dos avanzan según como se mueve el otro, también construyen muros para impedir el paso del otro, y 
así poder acorralar al enemigo y se le complique el paso. En el presente proyecto pensamos en un modo de cómo podemos mover la IA según la persona y hacerle difícil 
ganar o hasta hacer que pierda contra la IA. Como que, si los dos se encuentran a la misma distancia de llegar hasta el otro extremo, la IA piense si es más factible 
que se mueva o que ponga una pared para cortarle el paso sin que le juegue en contra a la IA, también se puede ver si la IA va perdiendo en pasos, le ponga paredes hasta 
que lo acorrale y el jugador tenga más pasos que dar para llegar hasta el otro extremo.