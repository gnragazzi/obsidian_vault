A diferencia de la [[Búsqueda-Árbol]], la ***Búsqueda-Grafo*** detecta y no admite estados repetidos
```
función BÚSQUEDA-GRAFO(problema, estrategia) retorna una solución o falla
	inicializar el árbol de búsqueda usando el estado inicial de problema
	inicializar el conjunto de nodos explorados en vacío
	while
		if (no hay candidatos para expansión) then return falla
		elegir un nodo hoja para expansión de acuerdo a estrategia¹
		if (el nodo contiene un estado objetivo) then return solución
		agregar el nodo al conjunto de nodos explorados
		expandir el nodo y agregar los nodos resultantes a la frontera² del árbol del búsqueda solamente si no está en la frontero o en el conjunto de nodos explorados³.
	FinWhile
FinFunción		
```
***
¹. A los efectos del caso, a este paso lo llamo evaluación de un nodo (primero se evalúa y después se expande)
². La frontera es la estructura de datos que se utiliza para almacenar los nodos.
³. ¿Se puede dar que un nodo esté en la frontera pero no en el conjunto de nodos explorados? #Dudas 