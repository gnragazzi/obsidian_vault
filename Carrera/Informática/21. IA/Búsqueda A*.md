- Evita expandir caminos que ya son suficientemente costosos
- La [[Búsqueda Primero el Mejor#^11b45a|Función de Evaluación]] es $f(n)=g(n)+h(n)$ donde
	- $g(n)$ es el costo para llegar a $n$. ([[Nodo de Árbol de Búsqueda - IA#^abb177|Función de Costo]]) 
	- [[Función Heurística - h(n)|h(n)]] 
	- $f(n)$ costo total *estimado* del camino más barato hasta el objetivo, que pasa por el nodo $n$
- Asegurando ciertas condiciones para $f(n)$ la búsqueda puede ser óptima y completa.
	- [[Admisibilidad]]´
	- [[Consistencia]] 
***
- Completa
	- Si, salvo que haya infinitos nodos $n$ tal que $f(n)≤f(G)$
- Tiempo
	- Exponencial en [error relativo en h × longitud de la solución]
- Espacio
	- Mantiene todos los nodos en memoria
- Óptima
	- Si
***
Observemos que ^efd71a
- $A^*$ expande todos los nodos $n$ con $f(n) < C^*$ (el costo óptimo)
- $A^*$ expande algunos nodos $n$ con $f(n) = C^*$ 
- $A^*$ no expande nodos $n$ con $f(n) > C^*$ 
***
[[Teorema Optimalidad de Búsqueda A*]] 