- Expande el nodo no expandido menos profundo
- El [[test de objetivo]] es realizado cuando el [[Nodo de Árbol de Búsqueda - IA|nodo]] es generado (antes de colocarlo en la [[Árbol de Búsqueda - Búsqueda IA#^92803d|frontera]])
***
Evaluación
- Completa — Si (si [[Estrategias de Búsqueda#^29acc8|b]] is finito)  
- Tiempo — $b + b^2 + b^3 + . . . + b^d = O(b^d)$, es decir, exp. en $d$ 
- Espacio — $O(b^d)$ (mantiene cada nodo en memoria en la ver. de [[Búsqueda-Grafo|grafo]]; en [[Búsqueda-Árbol|árbol]] podría generar menos pasos pero al tener redundantes el tiempo será problema!) 
- Óptima — Si, con costos de paso idénticos (o cualq. función no decreciente cra la prof.); no, en el caso general.

***
- ![[Pasted image 20250329164625.png]]
- ![[Pasted image 20250329164633.png]]
- ![[Pasted image 20250329164650.png]]