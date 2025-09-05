- $h(n)$ = estimación del costo de $n$ al *objetivo más cercano*
- $h(n)=0$ → $n$ es nodo objetivo.
***
Propiedades
- [[Admisibilidad]]
- [[Consistencia - Propiedad de Heurística (IA)]]
- [[Dominación - Heurísticas]]
***
Heurísticas admisibles pueden ser derivadas del costo exacto de una solución de una versión relajada del problema.
- Por ejemplo, si puedo volar desde un punto a otro en linea recta, se relaja el problema de encontrar el camino más corto entre 2 ciudades. De ello, se determina una heurística admisible
- Del ejemplo del 8-puzzle
	- Si las reglas del 8-puzzle son relajadas tal que una ficha se puede mover desde cualquier lugar, entonces $h_1(n)$ da la solución más corta.
	- Si las reglas son relajadas tal que una ficha se puede mover a cualquier cuadrado adyacente, entonces $h_2(n)$ da la solución más corta.
Punto clave: el costo de una solución óptima de un problema relajado no es mayor que el costo de la solución óptima del problema real.
[Algoritmos de Búsqueda Informados - Filmina 31] 