```
función BÚSQUEDA-ÁRBOL(problema, estrategia) retorna una solución o falla
	inicializar el árbol de búsqueda usando el estado inicial de problema
	while
		if (no hay candidatos para expansión) then return falla
		elegir un nodo hoja para expansión de acuerdo a estrategia¹
		if (el nodo contiene un estado objetivo) then return solución
		expandir el nodo y agregar los nodos resultantes a la frontera² del árbol del búsqueda
	FinWhile
FinFunción		
```
***
¹. A los efectos del caso, a este paso lo llamo evaluación de un nodo (primero se evalúa y después se expande)
². La frontera es la estructura de datos que se utiliza para almacenar los nodos.