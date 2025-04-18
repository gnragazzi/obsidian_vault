- Se quiere probar $q$ a partir de $BC$.
- Procedimiento: 
	- chequear si $q$ ya es conocido, o  
	- Si no, probar usando $BC$ todas las premisas de alguna regla que concluye $q$.
- Evitar loops
	- chequear si un nuevo subobjetivo ya está sobre el stack de objetivos.  
- Evitar trabajo repetido
	- chequear si un nuevo subobjetivo 
		- ya se ha demostrado que es verdadero, o  
		- ya ha fallado
***
- El encadenamiento hacia atrás es dirigido por el objetivo (goal-driven), apropiado para resolución de problemas.
***
Ejemplo:
- Base de Conocimiento:
	-  ![[Pasted image 20250418105128.png]]
- Grafo de conocimiento
	- ![[Pasted image 20250418105144.png]]
- ![[Pasted image 20250418110014.png]]
- ![[Pasted image 20250418110022.png]]
- ![[Pasted image 20250418110030.png]]
- etc