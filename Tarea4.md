# Practica 4 Introducción a la inteligencia artificial Introspección: Contar islas en una matriz.
## Introducción.
El siguiente ensayo abarca el planteamiento acerca de como resolver un problema que nos pide el contar el número de islas dentro de una matriz de elementos rectangulares o cuadrados utilizando dos metodos que son el iterativo y el recursivo. El objetivo del resolver dicho problema es para poner en práctica la autopercepción de nuestras mentes a la hora de encontrar la metodología o solucion adecuada para este problema. Es importante el reconocer la forma en que nuestra mente trabaja y como es que esta asocia los diferentes conocimientos previos para que podemos encontrar la forma más óptima de elaborar una solución para poder resolver un problema empleando las diferentes técnicas que se nos enseñaron durante la materia de inteligencia artificial.

## Desarrollo
El primer aspecto importante que hay que analizar del problema son las dimensiones de la matriz, en este caso es de 14 x 22 cuadros, que parecen tener mas bien formas rectangulares, dentro de dicha matriz se puede observar que la mayoría de los cuadros que la componen son de color o fondo blanco y se tienen 6 "islas" conformadas por cuadros de color gris oscuro, la diferencia de color nos muestra que elementos son los que hay que tener en cuenta y cual es el que se tiene que contar considerandolos "islas". Podemos resumir el problema como contar los cuadros de color gris, que serían los que contiene cada "isla" tomando en cuenta dos metodos, uno iterativo y uno recursivo en forma de algoritmos programados de los cuales se presentara el codigo. Para empezar podemos volverlo un problema separable al reconocer los dos estados, si es blanco la casilla entonces el programa devolveria un 0, si es gris devolveria un 1 siendo esta la forma de distinguirlos aunque aun existen un par de consideraciones mas que se deben de tener en cuenta pero se explicaran mas adelante con el desarrollo de los diversos metodos.

## Solucion con método iterativo.
Con el algoritmo iterativo se decidio emplear una función que fuera capaz de recorrer la matriz en el sentido de las filas y en cada fila una respectiva columna, mientras pasa con un valor numerico dependiendo del color de dicha casilla, en el caso de querer contar los elementos de color gris oscuro solo se haría referencia al número 1 como se establecio con anterioridad. Al recorrer cada posición, si el cuadro es blanco la referencia regresada por el programa sería un 0, esto empleando un contador auxiliar que nos ayude a referenciar cuando no se encontro una "isla". 
Usando como valores limites el tamaño de la propia matriz de 14x22, hacemos uso de una funcion iterativa que en este caso es un simple ciclo for bueno mas precisamente se usaran dos, con los cuales se podra recorrer fila y las columnas con el for anidado. Sin embargo existe otra consideracion mas que nos establece el problema y es que para poder contar las "islas" que estan contenidas en la matriz, las "islas" estan compuestas por varios elementos con valor 1 conectados entre si sea de forma vertical o horizontal. 
Por lo que si el programa encuentra un valor de 1, se debe de activar algun tipo de variable de control que indique que se están contando los elementos dentro de una sola isla por lo que se debe de guardar la posicion de las columnas en las que se encuentran los elementos identificados con 1 en dicha fila y luego continuar en la siguiente fila en el momento que se dejen de encontrar elementos que respondan al identificador 1, lo que se empleo es que después se recorre la siguiente fila específicamente en las columnas referenciadas para así ver si también hay elementos con valor 1 al tener que revisar en las cuatro direcciones. Aunque si hay otros elementos consecutivos en la misma fila, entonces estos también formarían parte de la isla, este proceso se realiza hasta llegar al punto en el que ya no haya elementos con identificador de 1 consecutivos y es entonces cuando a ese conjunto se le contaria como una isla. Después se repetiría el proceso principal para comprobar si dentro de la matriz existen mas islas.

## Ejemplo de solucion iterativa del problema:
```
matriz = [
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0],
[0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0],
[0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 0, 0],
[0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0],
[0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0],
[0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
[0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 1, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
]

filas = len(matriz)
columnas = len(matriz[0])

def busca_isla(matriz, f, c):
    if 0 <= f < filas and 0 <= c < columnas and matriz[f][c] == 1:
        matriz[f][c] = 0 
        busca_isla(matriz, f + 1, c)
        busca_isla(matriz, f - 1, c)
        busca_isla(matriz, f, c + 1)
        busca_isla(matriz, f, c - 1)

islas_encontradas = 0

for f in range(filas):
    for c in range(columnas):
        if matriz[f][c] == 1:
            islas_encontradas += 1
            explorar_isla(matriz, f, c)

print(f"El número total de islas encontradas en la matriz es: {islas_encontradas}")
```
Donde el color o elemento a contar seria el 1

## Solucion con método recursivo.
En el caso de una solucion recursiva el método empleado sería similar en la declaración de variables y contadores, pero este tendría que mandarse a llamar dentro de si mismo indicando las diferentes direcciones en las que podría moverse para encontrar la "isla" en base a la posición en la que se encuentre el programa, hay que considerar que si estamos en la posición 0 el programa no debe permitir ir a un número negativo y el límite sería ya sea el ancho o el alto de la matriz dependiendo de nuestra posicion, además si devolvemos un valor de 1 cuando vamos encontrando una isla se tiene la ventaja de que cuando se sume el contador podemos usar como referencia la propia recursividad del método utilizado.

## Ejemplo de solucion recursiva del problema:
```
def contarElementos(matriz, fila, columna, color):
    if not (0 <= fila < len(matriz)) or not (0 <= columna < len(matriz[0])) or matriz[fila][columna] != color:
        return 0

    contador = 1
    matriz[fila][columna] = None

    contador += contarElementos(matriz, fila + 1, columna, color)
    contador += contarElementos(matriz, fila - 1, columna, color)
    contador += contarElementos(matriz, fila, columna + 1, color)
    contador += contarElementos(matriz, fila, columna - 1, color)

    return contador

def contarIslas(matriz):
    islas_encontradas = 0

    for f in range(len(matriz)):
        for c in range(len(matriz[0])):
            if matriz[f][c] == 1:
                islas_encontradas += 1
                contarElementos(matriz, f, c, 1)

    return islas_encontradas

matriz = [
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0],
    [0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0],
    [0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 0, 0],
    [0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0],
    [0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0],
    [0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
    [0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 1, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
]

print(f"El número total de islas encontrados es: {contarIslas(matriz)}")
```

## Conclusión
En conclusión podemos apreciar como el método recursivo parece ser más óptimo que el iterativo aunque eso depende de que se considere como optimo ya que ambos metodos pueden adaptarse a distintas características que el otro según se necesite, por la naturaleza del problema considero que el recursivo tiene la ventaja dado que la conexión de los elementos que conforman una isla puede ser tanto de forma horizontal como vertical y el metodo recursivo nos permite seguir dentro de una misma funcion con cada comprobacion hacia una direccion. Lo que se puede observar en este ejercicio, es que teniendo asociados los métodos que vimos en las primeras clases de la materia con los ejercicios que estábamos resolviendo para encontrar islas también que se menciono al inicio de la materia, considero que entrando en contexto con la informacion sobre inteligencia artificial existen diversas caracteristicas y funciones de la misma que podrian sernos de ayuda para tratar de entrenar un modelo que lo hiciera de forma automatica.
