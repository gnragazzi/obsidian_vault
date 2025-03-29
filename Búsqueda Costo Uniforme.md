- Expande el nodo no que tiene menor costo de paso
- El [[test de objetivo]] es realizado cuando el [[Nodo de Árbol de Búsqueda - IA|nodo]] es seleccionado para la expansión (cuando se saca de la [[Árbol de Búsqueda - Búsqueda IA#^92803d|frontera]])
***
Evaluación (la complejidad toma en cuenta el costo del paso)
- Completa — Si, solo si el costo de cada paso $≥ ε$  (si [[Estrategias de Búsqueda#^29acc8|b]] is finito)  
- Tiempo — coincide con el de BPA cuando los costos de pasos son identicos. En general es $O(b^{\lceil{C^*/ε}\rceil})$ donde $C^*$ es el costo de la solución ótima y cada acción cuesta $≥ε$
- Espacio — Idem tiempo
- Óptima — Si, nodos expandidos incrementalmente en g(n).

***
- ![[Pasted image 20250329165200.png]]