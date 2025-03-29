Criterio para determinar el orden de expansión de los nodos. (Ordenar la [[Árbol de Búsqueda - Búsqueda IA#^92803d|Frontera]] de forma tal de expandir el primer nodo de la cola).
***
Se evalúan de acuerdo a las siguientes dimensiones:
- Completitud
	- Siempre encuentra una solución si dicha solución existe?
- Complejidad de tiempo
	- Cuánto tarda en encontrar una solución?
	- Medido en términos de número de nodos generados en la búsqueda
- Complejidad de espacio
	- Cuánto memoria necesita?
	- Medido en términos del máximo número de nodos almacenados en la memoria.
- Optimalidad
	- Siempre encuentra la mejor solución?
***
La complejidad es medida en términos de 
- $b$ factor de ramificación máximo del árbol ^29acc8
- $d$ profundidad del nodo objetivo menos profundo ^dcfff5
- $m$ profundidad máxima del espacio de estado (altura del árbol de búsqueda #Dudas ) ^ee214a
***
Existen 2 clasificaciones
1. [[Estrategias de Búsqueda no Informadas]]
2. [[Estrategias de Búsqueda Informadas]] 