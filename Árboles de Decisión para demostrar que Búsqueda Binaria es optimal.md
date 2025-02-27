Se pueden usar [[Árboles de Decisión (Decision Tree)|árboles de decisión]] para probar que dentro del [[Comparission_Based Model]], [[Binary Search]] es [[Complejidad e-c|optimal]]. 
- Cada nodo es una comparación.
- Todo árbol de decisión que modela algún algoritmo que resuelve el [[Búsqueda|problema de la búsqueda]] debe tener *al menos $n$ nodos* (caso contrario, habría comparaciones entre el elemento buscado y algún elemento de la lista que no se realizarían, y el algoritmo sería incorrecto para ciertas entradas).
- Viendo que 
	- ![[Pasted image 20250227082533.png]]
	- Donde el nodo raíz compara $X$ con el elemento en el medio de la lista, y determina uno de dos caminos posibles, o su hijo izquierdo o su hijo derecho, según si $X$ es menor o mayor, respectivamente. 
	- La comparación que hay en cada nodo es el punto de quiebre, donde se determina que rama seguir.
- 
***

