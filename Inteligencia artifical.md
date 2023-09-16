## Medida de rendimiento y frecuencia de percepcion para el problema de la lechuga, el pollo y el zorro

**Para este problema la medida de rendimiento es pasar a todos los individuos de uno en uno, utilizando el menor numero de viajes posibles y sin que se coman entre ellos ninguno de ellos**

| Posicion inicial | Barco | Posicion Final | Accion a realizar |
| --------- | --------- | --------- | --------- |
| ( L P Z ) | ( ) | ( ) | Llevarse al pollo |
| ( L Z ) | ( P ) | ( ) | Dejar al pollo y regresar por el zorro |
| ( L ) | ( Z ) | ( P ) | Dejar al zorro y regresar con el pollo |
| ( L ) | ( P ) | ( Z ) | Dejar al pollo y llevarse la lechuga |
| ( P ) | ( L ) | ( Z ) | Dejar la lechuga y ir por el pollo |
| ( ) | ( P ) | ( L, Z ) | Dejar al pollo  |
| ( ) | ( ) | ( P, L, Z ) | Fin |

## Medida de rendimiento y frecuencia de percepcion para el problema de los monjes y canibales

**Para este problema la medida de rendimiento es pasar a todos los individuos sea de uno en uno o pasando de dos en dos, utilizando el menor numero de viajes posibles, que la canoa siempre debe ser manejada por un individuo y que sin importar el movimiento nunca queden mas canibales que monjes en una de las orillas porque entonces los canibales se comerian a los monjes**

| Posicion inicial | Barco | Posicion Final | Accion a realizar |
| --------- | --------- | --------- | --------- |
| ( M M M C C C ) | ( ) | ( ) | Cruzar dos canibales |
| ( M M M C ) | ( C C ) | ( ) | Dejar a un canibal y regresar |
| ( M M M C ) | ( C ) | ( C ) | Irse los dos canibal |
| ( M M M ) | ( C C ) | ( C ) | Dejar a un canibal y regresar |
| ( M M M ) | ( C ) | ( C C ) | Dejar a un canibal y irse dos monjes |
| ( M C ) | ( M M ) | ( C C ) | Dejar a un monje y regresar uno y uno |
| ( M C ) | ( M C ) | ( M C ) | Dejar al canibal y irse los monjes |
| ( C C ) | ( M M ) | ( M C ) | Dejar a los monjes y regresar el canibal |
| ( C C ) | ( C ) | ( M M M ) | Llevarse otro canibal |
| ( C ) | ( C C ) | ( M M M ) | Dejar un canibal y regresar |
| ( C ) | ( C ) | ( M M M C ) | Llevarse al ultimo canibal |
| ( ) | ( C C ) | ( M M M C ) | Quedarse todos del otro lado |
| ( ) | ( ) | ( M M M C C C ) | Fin |

## Medida de rendimiento y frecuencia de percepcion para el problema de las ranas rojas y azules con un salto cada color

**Para este problema la medida de rendimiento es pasar a todos los individuos de un lado a otro, pero las ranas solo pueden saltar una a la vez, no pueden saltar mas de una rana o un espacio vacio, no pueden regresarse y deben saltar una rana azul y luego una roja y asi sucesivamente**

| Posiciones | Accion a realizar |
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
| No hay mas combinaciones | El problema no tiene solucion |

**Bajo la medida de rendimiento empleada con anterioridad es claro que el problema de las seis ranas no puede ser resuelto de esta forma dado que se atora de forma contundente sin importar que acciones se tomen, por ello a continuacion se va a replantear un punto en especifico empleado en la medida de rendimiento**

## Medida de rendimiento y frecuencia de percepcion para el problema de las ranas rojas y azules siendo capaz de saltar mas de un color seguido

**Para este problema la medida de rendimiento es pasar a todos los individuos de un lado a otro, pero las ranas solo pueden saltar una a la vez, no pueden saltar mas de una rana o un espacio vacio, no pueden regresarse y en este caso pueden saltar en cualquier orden**

| Posiciones | Accion a realizar |
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

