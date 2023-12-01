
# Practica 5 Introducción a la inteligencia artificial Introspección: Elementos de color en una imagen.
## Introducción
De manera digital las imágenes se han manejado tomando distintos espacios o píxeles a los que se les asigna un valor que es mostrado en monitor. Esto antes funcionaba de manera monocromática y permitía dibujar imágenes a partir de únicamente dos colores, dibujando en una matriz que sería la representación de la pantalla distintos valores que variarían entre 0 y 1 para mostrar la imagen al unirlos todos en una sola formación bidimensional que se mostraría a través de una interfaz, que en aquel tiempo únicamente podía hacer una pantalla.
Conforme se avanzó la tecnología fue capaz de manejarse valores de arreglos simples dentro de cada valor de esta matriz, estos valores serían la representación de colores más complejos a partir de unos principales, como es en el rgb tres valores y un Alfa que representa la opacidad. Así se podría dibujar una matriz donde cada valor tendría en sí un arreglo de tres valores o cuadros y se incluía el Alfa y estos a su vez generarían un promedio que dibujaría en una pantalla que permite hacer color una imagen con colores mucho más complejos que podrían variar de acuerdo a todas las combinaciones posibles de los valores en cada arreglo de cada pixel de cada imagen aumentando de una cantidad muy baja a una cantidad absurdamente grande de combinaciones y valores que ahora podrían representar distintas imágenes dentro de múltiples tipos de pantalla.
El problema planteado en esta sección en realidad es algo muy similar a lo anteriormente resuelto en una matriz simple solo que ahora se deberá manejar una matriz mucho más grande y darle al que se tendrá que diferenciar elementos que No necesariamente pueden ser valorados de un único modo y generando una igualdad específica a la que se tiene que buscar de modo que si antes teníamos que buscar Islas ahora lo que tenemos que buscar son segmentos con valores dentro de un Rango asociado promediando los valores dentro del arreglo de cada sección de la matriz principal.

## Desarrollo
La primera impresión que tengo de este problema es que veo una imagen con muchos objetos distribuidos y que además hay una gran variedad de colores. La mayoría de estos son alimentos que tienen tamaños, formas y colores distintos. Lo primero que se me viene a la mente en esta situación es que en un concepto muy básico una imagen puede ser considerada como una matriz, una matriz de pixeles, a fin de cuentas, en donde cada uno tiene un color distinto. 
Otra característica que observo es que la imagen es una matriz muy grande que, de hecho, su tamaño puede no siempre estar definido como lo es el caso de una matriz pequeña, pero a fin de cuentas si tomamos las medidas del número de filas y columnas entonces el ejercicio se puede resolver de manera muy similar al anterior, que es el de las islas, a fin de cuentas, en este caso es como si contáramos islas, pero ahora manejando un color como referencia. 
Para tener una referencia más clara y limitar los colores podríamos utilizar los rangos numéricos en que los colores se acercan a los tonos rojos y tener una sola referencia para detectar todos los objetos que puedan considerarse “rojos”. Los colores que normalmente hemos manejado en estos rangos son los RGB que son los tres colores primarios que forman a los demás, aunque solo es un formato de muchos que se manejan para el color digital. 
El primer paso sería poder procesar la imagen para convertirla en una matriz, esto utilizando una librería que permita el manejo de imágenes y colores como el caso de open cv del lenguaje Python, luego definir los colores. Además se debería definir un contador para guardar el número de elementos, objetos o islas encontrados con la característica que se solicita. Ejemplo de algoritmo.

```
r1 = 100, g1 = 0, b1 = 0
r2 = 255, g2 = 100, b2 = 100
islas = 0

mapa = cv.imread('atividad5.png', 1)  #leer los 3 canales con 1
w =mapa.shape[0]
h =mapa.shape[1]   #w y h para el ancho y alto de la imagen (filas y columnas)
#funcion para evaluar el color 
def rojo(i, j):
    if(mapa[i, j][2] >= r1 and mapa[i, j][2] <= r2):
        if(mapa[i, j][1] >= g1 and mapa[i, j][1] <= g2):
            if(mapa [i, j][0] >= b1 and mapa[i, j][0] <= b2):
                return True;
    return False;

Método recursivo. 
def metodoRecursivo(i, j):
    if not(i < 0 or i >= w or j < 0 or j >= h):
        if(rojo(i,j)):
            mapa[i,j][2] = 0
            mapa[i,j][1] = 0
            mapa[i,j][0] = 0
            metodoRecursivo(i - 1, j)
            metodoRecursivo(i + 1, j)
            metodoRecursivo(i, j - 1)
            metodoRecursivo(i, j + 1)
    return

Ejemplo iterativo: 
for i in range(w):
    for j in range(h):
        if(rojo(i, j)):
            islas += 1
            metodoRecursivo(i, j);
Mostrar resultados 
cv.imshow('Original',mapa)
print('islas:',islas)
cv.waitKey(0)
cv.destroyAllWindows()
```

## Conclusión
El ejemplo tratado es muy similar al anterior, donde solo se contaban islas, de hecho, entre más pequeños son los pixeles, más curveadas pueden apreciarse esas islas, pero viéndolos desde la perspectiva de una matriz, sabemos que también son cuadradas como el caso de una matriz que es más pequeña. Para el cerebro humano es más fácil detectar los objetos con colores porque no necesita hacer un análisis tan profundo del mismo, solo observa un todo en el que hay formas, colores, tamaños y diseños. En el caso de una computadora, esta tiene que aprender a procesar las imágenes como en este ejemplo, como si estas fueran una matriz y existen algunas librerías, como lo es open cv de Python que resultan muy útiles para el desarrollo de inteligencias artificial enfocada a la visión.


# Práctica 6. Introducción a la Inteligencia Artificial: El proceso de razonamiento según la lógica
## Problema
El Problema de Josephus se puede plantear matemáticamente como sigue: dado un círculo de n soldados numerados de 1 a n, y una constante k, los soldados son eliminados secuencialmente en pasos de k soldados, comenzando desde el soldado en la posición 1, y el proceso se repite hasta que solo queda un soldado. La pregunta es: ¿En qué posición inicial se debe colocar Josephus para ser el último sobreviviente?

## Solucion
El siguiente programa utiliza una lista para representar a los soldados y elimina secuencialmente a los soldados según las reglas del problema. La función ubicacion toma dos parámetros: el número total de soldados (n) y el proceso de eliminación (k). El resultado es la posición en la que Josephus debe sentarse para ser el último sobreviviente.

```
def ubicacion(n, k):
    soldados = list(range(1, n + 1))
    indice_soldado_actual = 0
    
    while len(soldados) > 1:
        # Calculamos el índice del soldado a eliminar
        indice_soldado_a_eliminar = (indice_soldado_actual + k - 1) % len(soldados)
        
        # Eliminamos al soldado
        soldados.pop(indice_soldado_a_eliminar)
        
        # Actualizamos el índice del soldado actual para el próximo ciclo
        indice_soldado_actual = indice_soldado_a_eliminar % len(soldados)
    
    return soldados[0]

n_soldados = 41
k_valor = 2
posicion_ganadora = ubicacion(n_soldados, k_valor)

print(f"Josephus debe sentarse en la posición {posicion_ganadora} para ser el último sobreviviente.")
```

# Práctica 7. Introducción a la Inteligencia Artificial: El papel de la heurística
## Definicion de heuristica 
Cuando buscamos resolver un problema de una complejidad considerable se puede volver complicado encontrar una solución óptima para este.
La manera en que encontramos soluciones generalmente Busca ser muy concreta o atacar el problema de manera que se entienda perfectamente cómo y de qué modo se puede llegar a la solución. Sin embargo, esto puedo incrementar demasiado la complejidad de la resolución al punto que deja de ser rentable o se vuelve muy ineficiente el encontrar una solución óptima.
Para muchos problemas la solución puede venir de varias maneras y aunque Generalmente existe una solución más óptima se puede resolver el problema de maneras menos eficientes pero más sencillas de pensar, existiendo soluciones comunes debido a la relativa simpleza con las que uno puede llegar a ellas a pesar de existir mejores soluciones.
Aquí es cuando el papel de la heurística se vuelve importante pues esta permite tomar un problema complejo y simplificarlo en uno que se puede resolver de manera más simple aunque sin buscar una solución concreta y eficiente, sino que tomando únicamente los elementos mínimos suficientes para poder resolver el problema en cuestión.
Así se puede llegar a soluciones bastante satisfactorias que además presentan un nivel de simpleza relativamente alto y que puede ser llevadas a cabo de manera aceptablemente eficiente aunque dejando el lugar para una solución más óptima.

## Solucion y algoritmo con recursividad programado
```
def Solucion(matriz, inicio, entrada):
    row, col = inicio
    num_rows, num_cols = len(matriz), len(matriz[0])

    if 0 <= row < num_rows and 0 <= col < num_cols:
        up_value = matriz[row - 1][col] if row - 1 >= 0 else float('inf')
        down_value = matriz[row + 1][col] if row + 1 < num_rows else float('inf')
        left_value = matriz[row][col - 1] if col - 1 >= 0 else float('inf')
        right_value = matriz[row][col + 1] if col + 1 < num_cols else float('inf')

        min_value = min(up_value, down_value, left_value, right_value)

        if min_value == up_value:
            movimiento = row - 1, col
        elif min_value == down_value:
            movimiento = row + 1, col
        elif min_value == left_value:
            movimiento = row, col - 1
        elif min_value == right_value:
            movimiento = row, col + 1
        
        if movimiento[0] == 0 or movimiento[0] == num_rows - 1:
            if  movimiento != entrada:
                return movimiento
        if movimiento[1] == 0 or movimiento[1] == num_cols - 1:
            if  movimiento != entrada:
                return movimiento
        
        matriz[row][col] += 0.1
        
        return Solucion(matriz, movimiento, entrada)

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

inicio = (7, 0)

end = Solucion(matriz, inicio, inicio)
print("Entrada: ", inicio, "\nSalida:  ", end)
```

## Explicacion
El funcionamiento del algoritmo sigue la solución propuesta y se adapta un código que sea ejecutable por Python.
El algoritmo al ser recursivo funcionará llamándose a sí mismo cada que encuentre un nuevo espacio. Lo primero es definir qué información necesita el algoritmo para funcionar, este requiere de una matriz que representará el espacio, un punto que indicará en dónde se encuentra en la matriz, y una coordenada que indica cuál es la entrada para utilizarla al momento de diferenciar la salida.
Este obtiene las coordenadas del punto en que se encuentra, además del tamaño que tiene la matriz. Después válida que el punto existe en la matriz y una vez hecho eso comienza a obtener los valores de los espacios que se encuentran una coordenada arriba, abajo, a la izquierda, y a la derecha, obteniendo después cuál es la coordenada del espacio que tiene el menor valor para así tomar este como el siguiente paso a dar.
Una vez hecho eso se obtendrá la coordenada de este nuevo espacio y se analizará que esta no sea una salida, de no serlo se volverá a llamar la función de manera recursiva pasando la matriz donde el valor de la coordenada por la que se acaba de pasar se aumentará en 0.1, se le pasará un nuevo punto de inicio qué será el espacio al que se deberá de mover y el mismo punto de entrada para que la pueda diferenciar de la salida.
Una vez hecho esto se le puede mandar una matriz inicial que posea un único cero en el borde y un camino recorrible donde la matriz puede tener cualquier tamaño y se respete los ceros y unos como representaciones de Laberinto. Este lo resolverá recorriéndolo para finalmente devolver el punto de entrada y el de salida.

# Practica 8 Reglas y Búsquedas : Espacio de Estados

## Medida de rendimiento y frecuencia de percepción para el problema de las ranas rojas y azules con un salto cada color

**Para este problema la medida de rendimiento es pasar a todos los individuos de un lado a otro, pero las ranas solo pueden saltar una a la vez, no pueden saltar mas de una rana o un espacio vació, no pueden regresarse y deben saltar una rana azul y luego una roja y así sucesivamente**

| Posiciones | Acción a realizar |
| --------- | --------- |
| ( A1 A2 A3 _ R1 R2 R3 ) | Salta rana azul 2|
| ( A1 _ A3 A2 R1 R2 R3 ) | Reiniciar porque no pueden seguir |
| ( A1 A2 A3 _ R1 R2 R3 ) | Salta rana azul 3|
| ( A1 A2 _ A3 R1 R2 R3 ) | Salta rana roja 1|
| ( A1 A2 R1 A3 _ R2 R3 ) | Salta rana azul 3|
| ( A1 A2 R1 _ A3 R2 R3 ) | Salta rana roja 2|
| ( A1 A2 R1 R2 A3 _ R3 ) | Salta rana azul 3|
| ( A1 A2 R1 R2 _ A3 R3 ) | Salta rana roja 3|
| ( A1 A2 R1 R2 R3 A3 _ ) | Salta rana azul 3|
| ( A1 A2 R1 R2 R3 _ A3 ) | Reiniciar porque no se puede seguir|
| No hay mas combinaciones | El problema no tiene solución |

**Bajo la medida de rendimiento empleada con anterioridad es claro que el problema de las seis ranas no puede ser resuelto de esta forma dado que se atora de forma contundente sin importar que acciones se tomen, por ello a continuación se va a replantear un punto en especifico empleado en la medida de rendimiento**

## Medida de rendimiento y frecuencia de percepción para el problema de las ranas rojas y azules siendo capaz de saltar mas de un color seguido

**Para este problema la medida de rendimiento es pasar a todos los individuos de un lado a otro, pero las ranas solo pueden saltar una a la vez, no pueden saltar mas de una rana o un espacio vació, no pueden regresarse y en este caso pueden saltar en cualquier orden**

| Posiciones | Acción a realizar |
| --------- | --------- |
| ( A1 A2 A3 _ R1 R2 R3 ) | Salta rana azul 3|
| ( A1 A2 _ A3 R1 R2 R3 ) | Salta rana roja 1|
| ( A1 A2 R1 A3 _ R2 R3 ) | Salta rana roja 2|
| ( A1 A2 R1 A3 R2 _ R3 ) | Salta rana azul 3|
| ( A1 A2 R1 _ R2 A3 R3 ) | Salta rana azul 2|
| ( A1 _ R1 A2 R2 A3 R3 ) | Salta rana azul 1|
| ( _ A1 R1 A2 R2 A3 R3 ) | Salta rana roja 1|
| ( R1 A1 _ A2 R2 A3 R3 ) | Salta rana roja 2|
| ( R1 A1 R2 A2 _ A3 R3 ) | Salta rana roja 3|
| ( R1 A1 R2 A2 R3 A3 _ ) | Salta rana azul 3|
| ( R1 A1 R2 A2 R3 _ A3 ) | Salta rana azul 2|
| ( R1 A1 R2 _ R3 A2 A3 ) | Salta rana azul 1|
| ( R1 _ R2 A1 R3 A2 A3 ) | Salta rana roja 2|
| ( R1 R2 _ A1 R3 A2 A3 ) | Salta rana roja 3|
| ( R1 R2 R3 A1 _ A2 A3 ) | Salta rana azul 1|
| ( R1 R2 R3 _ A1 A2 A3 ) | Fin |

## Medida de rendimiento y frecuencia de percepcion para el problema de la lechuga, el pollo y el zorro

**Para este problema la medida de rendimiento es pasar a todos los individuos de uno en uno, utilizando el menor numero de viajes posibles y sin que se coman entre ellos ninguno de ellos**

| Posicion inicial | Barco | Posicion Final | Acción a realizar |
| --------- | --------- | --------- | --------- |
| ( L P Z ) | ( ) | ( ) | Llevarse al pollo |
| ( L Z ) | ( P ) | ( ) | Dejar al pollo y regresar por el zorro |
| ( L ) | ( Z ) | ( P ) | Dejar al zorro y regresar con el pollo |
| ( L ) | ( P ) | ( Z ) | Dejar al pollo y llevarse la lechuga |
| ( P ) | ( L ) | ( Z ) | Dejar la lechuga y ir por el pollo |
| ( ) | ( P ) | ( L, Z ) | Dejar al pollo  |
| ( ) | ( ) | ( P, L, Z ) | Fin |

## Medida de rendimiento y frecuencia de percepción para el problema de los monjes y caníbales

**Para este problema la medida de rendimiento es pasar a todos los individuos sea de uno en uno o pasando de dos en dos, utilizando el menor numero de viajes posibles, que la canoa siempre debe ser manejada por un individuo y que sin importar el movimiento nunca queden mas caníbales que monjes en una de las orillas porque entonces los caníbales se comerían a los monjes**

| Posicion inicial | Barco | Posicion Final | Acción a realizar |
| --------- | --------- | --------- | --------- |
| ( M M M C C C ) | ( ) | ( ) | Cruzar dos caníbales |
| ( M M M C ) | ( C C ) | ( ) | Dejar a un caníbal y regresar |
| ( M M M C ) | ( C ) | ( C ) | Irse los dos caníbal |
| ( M M M ) | ( C C ) | ( C ) | Dejar a un caníbal y regresar |
| ( M M M ) | ( C ) | ( C C ) | Dejar a un caníbal y irse dos monjes |
| ( M C ) | ( M M ) | ( C C ) | Dejar a un monje y regresar uno y uno |
| ( M C ) | ( M C ) | ( M C ) | Dejar al caníbal y irse los monjes |
| ( C C ) | ( M M ) | ( M C ) | Dejar a los monjes y regresar el caníbal |
| ( C C ) | ( C ) | ( M M M ) | Llevarse otro caníbal |
| ( C ) | ( C C ) | ( M M M ) | Dejar un caníbal y regresar |
| ( C ) | ( C ) | ( M M M C ) | Llevarse al ultimo caníbal |
| ( ) | ( C C ) | ( M M M C ) | Quedarse todos del otro lado |
| ( ) | ( ) | ( M M M C C C ) | Fin |
