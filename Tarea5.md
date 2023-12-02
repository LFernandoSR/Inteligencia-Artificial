# Practica 5 Introducción a la inteligencia artificial Introspección: Elementos de color en una imagen.
## Introducción
El formato digital en las imágenes se ha manejado tomando distintos espacios o píxeles a los que se les asigna un valor, o varios dependiendo como RGB, que es mostrado en la pantalla en cuestion. En el pasado este tipo de funcionamiento era por lo que se conocia como monocromática y permitía dibujar diversas imágenes a partir de únicamente dos colores o mas bien un color y la ausencia de otro, dibujando en una matriz que sería la representación de la pantalla distintos valores que variarían entre 0 y 1 para mostrar la imagen al unirlos todos en una sola formación bidimensional que se mostraría a través de una interfaz, que en aquel tiempo únicamente podía hacer una pantalla.
Conforme paso el tiempo la tecnologia fue capaz de manejar valores mas complejos como arreglos y matrices, los valorees contenidos por este nuevo tipo de estructurras serían la representación de colores o mejor dicho espectros de colores más complejos a partir de unos principales, como ya se menciono el rgb que es la combinacion de tres valores y un Alfa que representa la opacidad. Así se podría dibujar una matriz donde cada valor tendría contenido un arreglo de tres valores o cuadros y se incluía el Alfa y estos a su vez generarían un promedio que dibujaría en una pantalla que permite hacer color una imagen con colores mucho más complejos que podrían variar de acuerdo a todas las combinaciones posibles de los valores en cada arreglo de cada pixel de cada imagen aumentando de una cantidad muy baja a una cantidad absurdamente grande de combinaciones y valores que ahora podrían representar distintas imágenes dentro de múltiples tipos de pantalla.
El problema planteado en esta practica o tarea mejor dicho en realidad es bastante similar al problema de las islas que fue resuelto con una matriz simple solo que en esta ocasion se deberá de emplear una matriz mucho más grande y considerar que se deben de diferenciar elementos que no necesariamente pueden ser valorados de un único modo como en el caso de las islas, y generando una igualdad específica a la que se tiene que buscar de modo que si antes teníamos que buscar Islas ahora lo que tenemos que buscar son segmentos con valores similares dentro de un Rango asociado promediando los valores dentro del arreglo de cada sección de la matriz principal.

## Desarrollo
A primera vista lo que podemos observar en la imagen asignada es que esta cuenta con una gran variedad de objetos distribuidos y que evidentemente estos cuentan con una variedad igual de grande de colores. La mayoría de los objetos de la imagen son alimentos que tienen tamaños, formas y colores distintos por lo que no se podria esperar encontrar un patron por ese lado. Retomando lo mencionado con anterioridad podemos partir de considerar a la imagen como una matriz de pixeles en donde cada uno tiene un color distinto que es lo que trataremos de identificar. 
Una caracteristica importante acerca de esta resolucion es que la imagen establecida en termino de matriz es considerablemente grande, ya que si se usa una imagen distinta su tamaño puede no siempre estar definido como lo es el caso de una matriz pequeña, pero si tomamos las medidas del número de filas y columnas entonces el ejercicio se puede resolver de manera muy similar al anterior, que es el de las islas solo que en este caso las islas serian el color de referencia o buscado.
El siguiente punto a considerar de este planteamiento es como limitar los colores que se tratan de identificar, para este caso se piensa utilizar los rangos numéricos en que los colores se acercan a los tonos rojos y tener una sola referencia para detectar todos los objetos que puedan considerarse “rojos”. Los colores o el espectro de colores empleados en estos rangos y para este problema son los establecidos por el modelo RGB que son los tres colores primarios que en su conjunto y grado forman a los demás. 
El primer paso es procesar la imagen que se le brinde al programa para convertirla en una matriz y asi poder llevar el conteo de las filas y columnas que la componen, esto por medio de una librería que nos permita el manejo de imágenes y colores como es el caso de open cv del lenguaje Python. Además se definio un contador para guardar el número de elementos, objetos o colores encontrados con la característica que se solicita. 

**Ejemplo de algoritmo.**
```
r1 = 100, g1 = 0, b1 = 0
r2 = 255, g2 = 100, b2 = 100
conjunto = 0

mapa = cv.imread('atividad2.png', 1) 
w =mapa.shape[0]
h =mapa.shape[1]  

def rojo(i, j):
    if(mapa[i, j][2] >= r1 and mapa[i, j][2] <= r2):
        if(mapa[i, j][1] >= g1 and mapa[i, j][1] <= g2):
            if(mapa [i, j][0] >= b1 and mapa[i, j][0] <= b2):
                return True;
    return False;

# Método recursivo. 
def mapeo(i, j):
    if not(i < 0 or i >= w or j < 0 or j >= h):
        if(rojo(i,j)):
            mapa[i,j][2] = 0
            mapa[i,j][1] = 0
            mapa[i,j][0] = 0
            mapeo(i - 1, j)
            mapeo(i + 1, j)
            mapeo(i, j - 1)
            mapeo(i, j + 1)
    return

for i in range(w):
    for j in range(h):
        if(rojo(i, j)):
            conjunto += 1
            mapeo(i, j);
# Mostrar resultados 
cv.imshow('Original',mapa)
print('conjuntos de color rojo:',conjunto)
cv.waitKey(0)
cv.destroyAllWindows()
```

## Conclusión
El problema abarcado en este trabajo es bastante similar al algoritmo presentado para el conteo de las islas y podemos notar como entre más pequeños son los pixeles, más curveadas pueden apreciarse esos conjuntos que presentan similitud, y si lo enfocamos desde la perspectiva de una matriz, nos damos cuenta que son cuadradas como el caso de una matriz. Para el cerebro humano es más fácil detectar los objetos con colores porque no necesita hacer un análisis tan profundo del mismo, solo observa un todo en el que hay formas, colores, tamaños y diseños. En el caso de una computadora, esta tiene que aprender a procesar las imágenes ya que no entiende a la misma como nosotros la entendemos por lo que se le tiene que especificar el detectarla como si la imagen fuera una matriz y existen algunas librerías, como lo es open cv de Python que resultan muy útiles para el desarrollo de inteligencias artificial enfocada a la visión de computadora, siendo el problema de esta ocasion un ejemplo muy pequeño de lo que se puede llegar a hacer.
