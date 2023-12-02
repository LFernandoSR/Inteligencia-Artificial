# Práctica 6. Introducción a la Inteligencia Artificial: El proceso de razonamiento según la lógica
## Problema
El Problema presentado en la actividad es de Josephus que podemos plantear matemáticamente de la siguiente forma: dado un círculo de n soldados numerados de 1 a n, y una constante k, los soldados son eliminados secuencialmente en pasos de k soldados, comenzando desde el soldado en la posición 1, y el proceso se repite hasta que solo queda un sobreviviente. La pregunta del problema es la siguiente: ¿En qué posición inicial se debe colocar Josephus para ser el último sobreviviente?

## Solucion
Se desarrollo un programa que utiliza una lista para representar a los soldados del problema y elimina secuencialmente a los soldados según las reglas del problema. La función principal toma dos parámetros: el número total de soldados (n) y el proceso de eliminación (k). El resultado es la posición en la que Josephus debe sentarse para ser el último sobreviviente de todos.
```
def posicion(n, k):
    soldados = list(range(1, n + 1))
    indice_soldado_actual = 0
    
    while len(soldados) > 1:
        indice_soldado_a_eliminar = (indice_soldado_actual + k - 1) % len(soldados)
        
        soldados.pop(indice_soldado_a_eliminar)
        
        indice_soldado_actual = indice_soldado_a_eliminar % len(soldados)
    
    return soldados[0]

n_soldados = 41
k_valor = 2
posicion_superviviente = posicion(n_soldados, k_valor)

print(f"Josephus debe sentarse en la posición {posicion_superviviente} para ser el último sobreviviente.")
```

## Conclusiones
En comparacion con los problemas anteriormente resueltos en las tareas previas este requeria de una solucion un poco mas sencilla y matematica debido a los valores iniciales, al no depender tanto de identificar valores sino de que ya se conocian el establecimiento de la solucion dependia principalmente del modelo que se empleara para resolver el problema. En este caso un simple proceso de elimiar y reubicar en un arreglo los valores que buscabamos nos permitio dar una solucion corta y sencilla al problema que aplica a conjuntos mas grandes siempre y cuando la caracteristica de ser inpar la gente total se mantenga.
