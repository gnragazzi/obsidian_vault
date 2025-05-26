Estructura de datos resultante de la aplicación del [[Búsqueda IA#^c92bac|proceso de búsqueda]].
Está compuesto por
- Raiz: [[Nodo de Árbol de Búsqueda - IA|nodo]] que corresponde al estado Inicial
- Hojas: Nodos que corresponden a estados que no tienen sucesores en el árbol
	- Todavía no fueron expandidos
	- Fueron expandidos y no tienen estados sucesores
***
La ***frontera del árbol de búsqueda*** es la estructura de datos que es una colección de estados que están esperando para ser expandidos. Se suele implementar como una [[Queue|Cola]]. El ordenamiento de la frontera dependerá de la [[Estrategias de Búsqueda]] que se utilice. ^92803d
***
Según se quieran detectar y evaluar o no los estados repetidos
1. [[Búsqueda-Árbol]] 
2. [[Búsqueda-Grafo]] 
***
**El espacio de estados no es igual al árbol de búsqueda**