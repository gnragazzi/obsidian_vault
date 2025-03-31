- Expande el nodo no expandido más profundo}
- [[Árbol de Búsqueda - Búsqueda IA#^92803d|Frontera]]: cola LIFO ([[Pila - Stack]]), es decir, coloca sucesores al frente.
***
Evaluación
- Completa
	- En grafo: completa en espacios finitos
	- En árbol: no completa (en espacios con loop)
- Tiempo
	- $O(b^m)$, terrible si [[Estrategias de Búsqueda#^ee214a|m]] es más grande que [[Estrategias de Búsqueda#^dcfff5|d]]. 
- Espacio
	- Árbol: $O(bm)$ es decir, es lineal en espacio (solo se necesita almacenar un único paso desde la raiz al nodo hoja). 
	- Para el caso de grafo, igual que tiempo y que bpa. 
	- No
***
![[Pasted image 20250329165816.png]]