#### Definición
- Es la capacidad de volver al estado coherente más reciente previo a un fallo. Esto implica que el sistema debe mantener suficiente información para lograr recuperarse de los fallos y recuperar la información
- El sistema debe hacer un seguimiento de cuando se inicia, termina, confirma y/o aborta una transacción. Es decir, de las operaciones:
	- BEGIN
	- READ
	- WRITE
	- COMMIT
	- ROLLBACK
- Una forma de lograr esto es mantener una bitacora (logs) para mantener información detallada sobre los cambios realizados
	- Si hay daños físicos, debido a fallos catastróficos, se recupera a partir del último backup repitiendo las transacciones a partir del punto de recuperación
	- Si no hay daños físicos, es decir si los fallos son no-catastróficos pero la BD se encuentra en un estado inconsistente, se revierten los cambios que introdujeron la inconsistencia deshaciendo algunos cambios recientes.
	- [[Ejemplo logs Recuperación BD]]

***
#### Etiquetas
- #Anki 