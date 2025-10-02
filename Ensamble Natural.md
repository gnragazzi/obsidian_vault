#### Definición
- Esta operación realiza el ensamblaje de tuplas por atributos comunes con iguales valores.
	- ![[Pasted image 20250928194055.png|300]]
- Si no hay índices, el costo es el costo de ensamblaje
- Si hay índice en una de las relaciones, por el atributo de ensamble, se recorre secuencialmente la relación sin el índice y por cada tupla se busca en la relación con el índice, usandolo.
	- MP: O(N* costo del índice)
	- I/O: O(N/b* costo del índice)
***
#### Etiquetas
- #Anki 