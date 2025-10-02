#### Costo de Implementación de $\Pi_X(r)$
- Si una de las claves está incluida en X
	- Hay tantas instancias como nuplas en $r$
	- Costos
		- Accesos a MP $O(N)$ 
		- (I/O) $O(N/b)$
			- donde b es el número de nuplas por página de disco
- Si no hay clave incluida en X
	- Habrá nuplas repetidas, así que se necesitará un algoritmo de ordenamiento para eliminarlas
		- En SQL no se eliminan repetidas salvo explicitamente hacerlo con DISTINCT
	- Costos
		- Accesos a MP $O(N\;\log\; N)$
		- Accesos a disco (con ordenamiento) [[Costos del Problema de Ordenamiento]]
	
***
#### Etiquetas
- #Anki 