Define una dependencia de uno a muchos entre objetos, de manera que cuando el estado de un objeto cambia, todas las dependencias se notifican y son actualizados automáticamente.
***
Hay dos [[Interfaz - OOP|Interfaces]] y dos clases concretas:
- La interfaz *Subject* con métodos:
	- Para registrar un nuevo observador
	- para remover un observador
	- Para notificar observadores cuando el estado cambia
- La clase concreta que implementa *subject*
	- Que debe tener una lista de observadores y un estado
- La Interfaz *Observer* con método
	- update - para realizar los cambios necesarios cuando recibe una actualización del *Subject*
- El observador concreto 
	- **Que debe tener registro del su** ***subject*** .
***
Principios de diseño que aplica:
- [[Principio de Diseño 4 - Bajo Acoplamiento]]
- [[Principio de Diseño 8 - Principio Hollywood]]
	- Porque el observador se comunica con el sujeto cuando tiene algo que decir, pero no al revés (esto cuando la actualización es *push* y no *pull*)
***
![[Pasted image 20250114095759.png]]
***
[[Implementación JAVA de Observer]]
