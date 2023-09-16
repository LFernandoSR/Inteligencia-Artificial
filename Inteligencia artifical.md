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

