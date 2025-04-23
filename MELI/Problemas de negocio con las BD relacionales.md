- Problemas de alta Disponibilidad
	- No son [[Sistemas Distribuidos|sistemas distribuidos]], sino más bien centralizados, lo que puede llevar a un Single Point of Failure.
- Las BD relacionales no escalan horizontalmente (a nivel de escritura). [[Diferencias entre SQL y NoSQL#^4c231e|Escalabilidad]]
- Modelar Objetos JSON en una BD relacional es rígido.
	- Los objetos JSON se han vuelto el estándar para cambiar intercambiar datos por internet.
	- Si un objeto JSON cambia, por ejemplo, lo hace también el proceso de mapeado de ese JSON a las entidades; además de llevar a cambios en las estructuras y relaciones.
	- Es decir que una BD NoSQL 
***
