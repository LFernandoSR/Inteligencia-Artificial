# Práctica 7. Introducción a la Inteligencia Artificial: El papel de la heurística
## El papel de la heuristica 
La manera en que generalmente encontramos soluciones a nuestros problemas busca ser de una manera concreta o atacar el problema de manera que se entienda perfectamente cómo y de qué modo se puede llegar a la solución de dicho problema. Sin embargo, esto puedo incrementar demasiado la complejidad de la resolución al punto que deja de ser rentable o se vuelve muy ineficiente el encontrar una solución óptima llegando a tener soluciones complicadas a un problema que en principio resulta simple.
Cuando buscamos resolver un problema de una complejidad considerable se puede volver complicado encontrar una solución óptima para este debido a los diversos factores que interfieren en el problema y la propia percepcion que tenga el individuo a la hora de afrontarlo.
Para muchos problemas la solución puede venir de varias maneras y aunque generalmente existe una solución más óptima para la resolucion del mismo cierto es que se puede resolver el problema de maneras menos eficientes pero más sencillas de pensar en menor tiempo, existiendo soluciones comunes basandose en la relativa simpleza con las que uno puede llegar a dichos resultados a pesar de existir teoricamente mejores soluciones.
Es en estas situaciones cuando el papel de la heurística toma una mayor importancia pues esta nos permite tomar un problema complejo y simplificarlo en uno que se puede resolver de manera más simple aunque sin buscar una solución concreta y eficiente, sino que tomando únicamente los elementos mínimos suficientes para poder resolver el problema en cuestión. Es decir busca dividirlo en partes mas sencillas de resolver.
De este modo es que se puede llegar a soluciones bastante satisfactorias que además presentan un nivel de simpleza relativamente alto y que puede ser llevadas a cabo de manera considerablemente eficiente aunque dejando el lugar para una solución más óptima. Pero la solucion que se busque depende de las propias condiciones del problema y el individuo ya que no siempre una solucion mas rapida es mejor o se ocupa una solucion mas rapida que una optima.
En este caso se nos presento un problema en el que en base a un laberinto dado siendo las paredes 1 y los caminos transitables un 0 debiamos de establecer un algoritmo y codigo que encontrara el camino a seguir.

## Solucion y algoritmo con recursividad
```
def Solucion(matriz, inicio, entrada):
    row, col = inicio
    num_rows, num_cols = len(matriz), len(matriz[0])

    if 0 <= row < num_rows and 0 <= col < num_cols:
        valor_arriba = matriz[row - 1][col] if row - 1 >= 0 else float('inf')
        valor_abajo = matriz[row + 1][col] if row + 1 < num_rows else float('inf')
        valor_izquierda = matriz[row][col - 1] if col - 1 >= 0 else float('inf')
        valor_derecha = matriz[row][col + 1] if col + 1 < num_cols else float('inf')

        min_value = min(valor_arriba, valor_abajo, valor_izquierda, valor_derecha)

        if min_value == valor_arriba:
            avance = row - 1, col
        elif min_value == valor_abajo:
            avance = row + 1, col
        elif min_value == valor_izquierda:
            avance = row, col - 1
        elif min_value == valor_derecha:
            avance = row, col + 1
        
        if avance[0] == 0 or avance[0] == num_rows - 1:
            if  avance != entrada:
                return avance
        if avance[1] == 0 or avance[1] == num_cols - 1:
            if  avance != entrada:
                return avance
        
        matriz[row][col] += 0.1
        
        return Solucion(matriz, avance, entrada)

    return None

matriz = [
    [1, 1, 1, 1, 1, 1, 1, 1, 1],
    [0, 0, 0, 0, 0, 0, 1, 0, 1],
    [1, 1, 1, 0, 1, 1, 1, 0, 1],
    [1, 0, 0, 0, 1, 0, 1, 0, 1],
    [1, 0, 1, 1, 1, 0, 1, 0, 1],
    [1, 0, 0, 0, 0, 0, 0, 0, 1],
    [1, 0, 1, 1, 1, 0, 1, 0, 1],
    [0, 0, 1, 0, 0, 0, 1, 0, 1],
    [1, 1, 1, 1, 1, 1, 1, 1, 1],
]

inicio = (8, 0)

end = Solucion(matriz, inicio, inicio)
print("La entrada del laberinto es: ", inicio, "\nLa salida del laberinto es:  ", end)
```

## Explicacion
El funcionamiento del algoritmo para la resolucion del laberitmo sigue la solución propuesta y se adapta un código que sea ejecutable por Python como los casos de tareas anteriores.
El algoritmo al ser de tipo recursivo funcionará llamándose a sí mismo cada que encuentre un nuevo espacio al cual puede moverse. Lo primero que se define es qué información obtiene el algoritmo para funcionar, este emplea una matriz que representará el espacio, un punto que indicará en dónde se encuentra en dicha matriz, y una coordenada que indica cuál es la entrada para utilizarla al momento de diferenciar la salida dado que en un laberinto uno no debe de salir por donde entro.
Este programa obtiene las coordenadas del punto en que se encuentra, además del tamaño que tiene la matriz. Después válida el punto existe en la matriz y una vez hecho eso comienza a obtener los valores de los espacios que se encuentran una coordenada arriba, abajo, a la izquierda, y a la derecha, obteniendo después cuál es la coordenada del espacio que tiene el menor valor para así tomar este como el siguiente paso a dar.
Una vez hecho eso se obtendrá la coordenada de este nuevo espacio y se analizará que esta no sea una salida, de no serlo se volverá a llamar la función de manera recursiva pasando la matriz donde el valor de la coordenada por la que se acaba de pasar se aumentará en 0.1, se le pasará un nuevo punto de inicio qué será el espacio al que se deberá de mover y el mismo punto de entrada para que la pueda diferenciar de la salida.
Una vez hecho esto se le puede mandar una matriz inicial que posea un único cero en el borde y un camino recorrible donde la matriz puede tener cualquier tamaño y se respete los ceros y unos como representaciones de Laberinto. Este lo resolverá recorriéndolo para finalmente devolver el punto de entrada y el de salida.
Cabe considerar que esto depende de que los bordes del laberinto se encuentren cerrados o con valor de 1 y solo existan una salida y una entrada o entonces el algoritmo empezara a realizar cosas raras. Otro punto a considerar es que nosotros debemos establecer la posicion inicial y entender que el camino que tome podria variar dependiendo de los propios limites que nosotros le pongamos de forma manual al sistema.
Ademas el programa presentado nos devuelve la salida del laberinto y su entrada no es que devuelva todo el camino y el mas optimo solo encuentra el camino de salida desde la entrada proporcionada.
