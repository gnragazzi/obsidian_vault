- En este caso, $f(n)=h(n)$[1]
- Expande el nodo que *parece* estar más cerca del objetivo.
***
- Completa
	- No, puede caer en loops
	- Si en espacio finito con chequeo de estado repetido ([[Búsqueda-Grafo]])
- Tiempo
	- $O(b^m)$
- Espacio 
	- $O(b^m)$ porque mantiene todos los nodos en memoria
- Óptima
	- No. (ver ejemplo).
***
Ejemplo:
$h_{DLR}(n)$ es una función que mide la distancia en linea recta desde un nodo al otro
![[Pasted image 20250329180212.png]]
![[Pasted image 20250329180222.png]]
Que no es la mejor opción, porque desde Sibiu se llega a bucarest con menos costo por Rimnicu Vilcea (aunque *parezca* peor opción por está más lejos en linea recta) que por Fagaras.
***
[1]. [[Función Heurística - h(n)|h(n)]] // [[Búsqueda Primero el Mejor#^11b45a|f(n)]] 
