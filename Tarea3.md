# Practica 3 Introducción a la inteligencia artificial Introspección
## Introducción
En este ensayo se aborda el como resolver un desafío, el cual consiste en intercambiar la posición de 4 alfiles blancos y 4 negros que se encuentran en la primera y última fila respectivamente en un tablero de ajedrez de dimensiones 5 x 4, la idea del ejercicio es interpretar la mejor solución desde el punto de vista introspectivo. 
La finalidad de este ensayo es conocer o tener un mejor entendimiento del proceso cognitivo y de resolución de problemas que se aplicaria a la inteligencia artificial basandonos en lo que tenemos los seres humanos, la inteligencia artificial pretende funcionar de la misma manera o muy cercana por lo menos a la inteligencia "natural" del ser humano.

## Desarrollo
**Análisis del problema.**
En primer lugar, podemos observar que el tablero tiene 5 filas y 4 columnas, la primera y la última fila son las únicas que tienen alfiles respectivamente, la fila superior tiene 4 alfires blancos y la fila inferior tiene 4 alfires negros. Conociendo las reglas basicas del juego del ajedrez podemos establecer que los alfiles solo pueden realizar movimientos en forma diagonales, por lo que la única manera de cambiarlos de posición es moverlos en el tablero de esa forma sin que colisionen entre si o con otro alfil. 
Las diagonales como en el ajedrez, pueden ser de 1 a n cuadros, aunque tomando en cuenta los detalles del tablero lo maximo que podria moverse dependeria de su posicion inicial. Si queremos evitar que esten dentro del campo de accion del resto de los afiles entonces podemos ver que estos no se pueden mover en una diagonal de distancia mayor a 2 cuadros, debido a que si exceden esta distancia entonces se encontrarian en los posibles caminos de los alfiles que se encuentran en el extremo opuesto.

**Estrategia inicial**
Debido a la naturaleza del problema hay cierta informacion que nos presentan los propios datos iniciales, uno no debe adelantarse a realizar movimientos apresurados cuando al hacer cuentas el tablero de 5x4 es un numero par y la cantidad de alfiles con los que se cuenta en un inicio tambien es un numero par por lo que lo mas probable es que la solucion tenga cierta simetria y funcione como un espejo un lado con el otro. Al intentar mantener dicha simetría, lo que hice fue empezar a mover los alfiles de la fila superior de la misma forma, pero como espejo, es decir, simétricamente inverso con respecto a la fila inferior del tablero. Avanzando de esta forma se llega a un punto en el que se debia de regresar a la primera fila al primer alfil blanco y al negro para poder repetir otro patrón de simetría de ambos lados con otros alfiles y que de esa manera quedara el camino libre para que los demás alfiles lograran moverse libremente.

**Movimientos**
Al mantener la simetria de los movimientos somos capaces de mover de forma adecuada y uno a uno los alfiles de los dos colores, entre los diversos casos con los que nos encontrabamos es que existian ocasiones en las que se debia de mover un solo cuadro de distancia en una direccion y otras en las que se desplazaba tres, siendo que la cantidad de desplazamiento de los alfiles terminaba por repetirse junto con la simetria. 
Llegando a los últimos movimientos realizados para el ejercicio nos quedaban diagonales en los extremos del tablero, por ejemplo, en la fila de hasta abajo (donde inicialmente se encontraban los alfiles blancos), quedaban dos diagonales de alfiles negros y en el otro lado el mismo caso, pero del color contrario manteniendo la debida simetria. Al ver esto me percaté que solo faltaban 2 movimientos respectivamente para cada color, es decir, 4 movimientos en total y se llegaba a la solución. 
Cada vez que un alfil blanco hacia un movimiento, la mejor estrategia era hacer que el siguiente alfil negro hiciera un movimiento similar, pero de forma de espejo, fue así como llegué a la solución. El número total de movimientos requeridos para llegar a la solucion del problema se muestran a continuacion en tablas.

| B1 | B2 | B3 | B4 |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| ** | ** | ** | ** |
| ** | ** | ** | ** |
| N1 | N2 | N3 | N4 |

| B1 | B2 | B3 | B4 |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| ** | ** | ** | ** |
| ** | ** | N2 | ** |
| N1 | ** | N3 | N4 |

| B1 | B2 | ** | B4 |
| -- | -- | -- | -- |
| ** | B3 | ** | ** |
| ** | ** | ** | ** |
| ** | ** | N2 | ** |
| N1 | ** | N3 | N4 |

| B1 | B2 | ** | B4 |
| -- | -- | -- | -- |
| ** | B3 | ** | N1 |
| ** | ** | ** | ** |
| ** | ** | N2 | ** |
| ** | ** | N3 | N4 |

| B1 | B2 | ** | ** |
| -- | -- | -- | -- |
| ** | B3 | ** | N1 |
| ** | ** | ** | ** |
| B4 | ** | N2 | ** |
| ** | ** | N3 | N4 |

| B1 | B2 | ** | ** |
| -- | -- | -- | -- |
| ** | B3 | ** | N1 |
| ** | ** | ** | ** |
| B4 | N3 | N2 | ** |
| ** | ** | ** | N4 |

| B1 | ** | ** | ** |
| -- | -- | -- | -- |
| ** | B3 | B2 | N1 |
| ** | ** | ** | ** |
| B4 | N3 | N2 | ** |
| ** | ** | ** | N4 |

| B1 | ** | ** | ** |
| -- | -- | -- | -- |
| N2 | B3 | B2 | N1 |
| ** | ** | ** | ** |
| B4 | N3 | ** | ** |
| ** | ** | ** | N4 |

| B1 | ** | ** | ** |
| -- | -- | -- | -- |
| N2 | ** | B2 | N1 |
| ** | ** | ** | ** |
| B4 | N3 | ** | B3 |
| ** | ** | ** | N4 |

| B1 | ** | N1 | ** |
| -- | -- | -- | -- |
| N2 | ** | B2 | ** |
| ** | ** | ** | ** |
| B4 | N3 | ** | B3 |
| ** | ** | ** | N4 |

| B1 | ** | N1 | ** |
| -- | -- | -- | -- |
| N2 | ** | B2 | ** |
| ** | ** | ** | ** |
| ** | N3 | ** | B3 |
| ** | B4 | ** | N4 |

| B1 | ** | N1 | ** |
| -- | -- | -- | -- |
| N2 | ** | B2 | ** |
| N3 | ** | ** | ** |
| ** | ** | ** | B3 |
| ** | B4 | ** | N4 |

| B1 | ** | N1 | ** |
| -- | -- | -- | -- |
| N2 | ** | ** | ** |
| N3 | ** | ** | B2 |
| ** | ** | ** | B3 |
| ** | B4 | ** | N4 |

| B1 | ** | N1 | ** |
| -- | -- | -- | -- |
| N2 | ** | ** | ** |
| N3 | ** | B3 | B2 |
| ** | ** | ** | ** |
| ** | B4 | ** | N4 |

| B1 | ** | N1 | ** |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| N3 | N2 | B3 | B2 |
| ** | ** | ** | ** |
| ** | B4 | ** | N4 |

| B1 | ** | N1 | ** |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| ** | N2 | B3 | B2 |
| ** | ** | ** | ** |
| ** | B4 | N3 | N4 |

| B1 | B2 | N1 | ** |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| ** | N2 | B3 | ** |
| ** | ** | ** | ** |
| ** | B4 | N3 | N4 |

| B1 | B2 | N1 | N2 |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| ** | ** | B3 | ** |
| ** | ** | ** | ** |
| ** | B4 | N3 | N4 |

| B1 | B2 | N1 | N2 |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| ** | ** | ** | ** |
| ** | ** | ** | ** |
| B3 | B4 | N3 | N4 |

| B1 | B2 | N1 | N2 |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| ** | N4 | ** | ** |
| ** | ** | ** | ** |
| B3 | B4 | N3 | ** |

| ** | B2 | N1 | N2 |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| ** | N4 | B1 | ** |
| ** | ** | ** | ** |
| B3 | B4 | N3 | ** |

| ** | B2 | ** | N2 |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| N1 | N4 | B1 | B4 |
| ** | ** | ** | ** |
| B3 | ** | N3 | ** |

| ** | B2 | ** | N2 |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| N1 | ** | B1 | B4 |
| N4 | ** | ** | ** |
| B3 | ** | N3 | ** |

| ** | B2 | ** | N2 |
| -- | -- | -- | -- |
| ** | ** | ** | B1 |
| N1 | ** | ** | B4 |
| N4 | ** | ** | ** |
| B3 | ** | N3 | ** |

| ** | B2 | ** | N2 |
| -- | -- | -- | -- |
| ** | ** | ** | B1 |
| N1 | ** | ** | B4 |
| N4 | ** | ** | N3 |
| B3 | ** | ** | ** |

| ** | ** | ** | N2 |
| -- | -- | -- | -- |
| B2 | ** | ** | B1 |
| N1 | ** | ** | B4 |
| N4 | ** | ** | N3 |
| B3 | ** | ** | ** |

| N3 | ** | ** | N2 |
| -- | -- | -- | -- |
| B2 | ** | ** | B1 |
| N1 | ** | ** | B4 |
| N4 | ** | ** | ** |
| B3 | ** | ** | ** |

| N3 | ** | ** | N2 |
| -- | -- | -- | -- |
| ** | ** | ** | B1 |
| N1 | ** | ** | B4 |
| N4 | ** | ** | ** |
| B3 | ** | ** | B2 |

| N3 | ** | ** | N2 |
| -- | -- | -- | -- |
| ** | N1 | ** | B1 |
| ** | ** | ** | B4 |
| N4 | ** | ** | ** |
| B3 | ** | ** | B2 |

| N3 | ** | ** | N2 |
| -- | -- | -- | -- |
| ** | N1 | ** | B1 |
| ** | ** | ** | ** |
| N4 | ** | B4 | ** |
| B3 | ** | ** | B2 |

| N3 | ** | ** | N2 |
| -- | -- | -- | -- |
| ** | N1 | N4 | B1 |
| ** | ** | ** | ** |
| ** | ** | B4 | ** |
| B3 | ** | ** | B2 |

| N3 | ** | ** | N2 |
| -- | -- | -- | -- |
| ** | N1 | N4 | ** |
| ** | ** | ** | ** |
| ** | B1 | B4 | ** |
| B3 | ** | ** | B2 |

| N3 | N4 | ** | N2 |
| -- | -- | -- | -- |
| ** | N1 | ** | ** |
| ** | ** | ** | ** |
| ** | B1 | B4 | ** |
| B3 | ** | ** | B2 |

| N3 | N4 | ** | N2 |
| -- | -- | -- | -- |
| ** | N1 | ** | ** |
| ** | ** | ** | ** |
| ** | ** | B4 | ** |
| B3 | ** | B1 | B2 |

| N3 | N4 | N1 | N2 |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| ** | ** | ** | ** |
| ** | ** | B4 | ** |
| B3 | ** | B1 | B2 |

| N3 | N4 | N1 | N2 |
| -- | -- | -- | -- |
| ** | ** | ** | ** |
| ** | ** | ** | ** |
| ** | ** | ** | ** |
| B3 | B4 | B1 | B2 |

## Conclusión
Para la resolución exitosa de este problema se requiere de una estrategia con un enfoque cuidadosamente definido desde el inicio del problema que se pueda utilizar para respetar las limitaciones impuestas por el juego, una de ellas es que cada color tenía que tomar un turno en cada movimiento no mover dos veces el negro o el blanco. Si lo vemos desde ese punto de vista los alfiles blancos tenian que intercambiar posiciones con los alfiles negros sin entrar en los rangos de ataque de los otros colores. En lo personal me fue algo dificil el interpretar las estrategias que realizo de forma mentar o escribirlos de forma coherente en una libre, considero que la forma en la que llego a la solución de algún problema es, ya sea simulándolo o haciendo los movimientos de forma grafica y necesito apoyarme de algun tipo de bitácora o lista para poder recordar los pasos que se han tomado hasta ese punto, como lo fué en este caso anotar en una hoja de papel y despues pasarlo a digital en formato markdown.
En conclusión, puedo afirmar que para solucionar un problema de esta indole lo primero que se debe observar detenidamente es el tablero del juego y las piezas que hay en dicho tablero, cuáles son sus dimensiones o tamaño del tablero, observar cuales son las reglas y las limitaciones para hacer los movimientos por parte de los alfiles, y en base a ello se puede deducir que si los movimientos eran alternados tenían que tener cierta coordinación y simetría al asociarlo con un numero par, además de que el número de piezas al ser par y de la misma cantidad en colores pues mantenia cierta lógica, también es importante tomar en cuenta los patrones que se van construyendo conforme se esta realizando el ejercicio ya, creo que teniendo en cuenta que estas características puede ser una herramienta útil para resolver otro problemas similares en un futuro.
