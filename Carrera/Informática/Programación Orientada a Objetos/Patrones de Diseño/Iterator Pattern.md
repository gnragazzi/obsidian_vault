Proveé una forma de acceder a los elementos de un [objeto agregado]¹ secuencialmente sin exponer su representación subyacente.
***
![[Pasted image 20250220082133.png]]
***
Al quitar la responsabilidad de las iteraciones del objeto y delegarlas en el iterator se permite usar el polimorfismo (sobrecarga).[Head First Design Patterns]
***
Principios de diseño que cumple:
- [[Principio de Diseño 1 - Encapsular lo que cambia]]_
	- Porque encapsulamos la forma en que un cliente itera sobre una colección, de modo que si hay que cambiar eso (o el cliente) todo se encuentra encapsulado.
- [[Principio de Diseño 2 - Programar a la interfaz]]
	- Porque trasladamos la funcionalidad de iterar del agregado al Iterator utilizando interfaces, tanto del agregado como del Iterador, de manera de que el cliente desconozca los detalles de implementación de ambos.
- [[Principio de Diseño 3 - Favorecer la composición a la herencia]]
	- Porque el agregado concreto esta compuesto por el iterator y utilizamos la herencia para crear la funcionalidad
- [[Principio de Diseño 4 - Bajo Acoplamiento]]
	- Es el caso del cliente, que no conoce detalles de implementación del agregado
- [[Principio de Diseño 9 - Principio de la Responsabilidad Única]]
	- Separamos las responsabilidades: la del agregado es controlar la colección de elementos, la del Iterator es iterar.

***
¹. Un objeto agregado es una colección de objetos utilizando alguna estructura de datos (arrayList, Hashtable, Array, etc).