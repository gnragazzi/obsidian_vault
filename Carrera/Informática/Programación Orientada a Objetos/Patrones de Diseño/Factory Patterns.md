Todos los patrones Factory encapsulan la creación de objetos.
1. [[Factory Method]]
2. [[Abstract Factory]]
***
Las diferencias entre estos dos patrones de diseño son:
- Factory method provee una interfaz abstracta para encapsular la creación de **un** producto, mientras que abstract factory lo hace para la creación de una familia de productos.
- FM utiliza herencia, mientras que AF utiliza composición

***
Principios de diseño que aplica:
- [[Principio de Diseño 1 - Encapsular lo que cambia]]
- [[Principio de Diseño 2 - Programar a la interfaz]]
- [[Principio de Diseño 3 - Favorecer la composición a la herencia]]
- [[Principio de Diseño 9 - Principio de la Responsabilidad Única]]
	- Porque separa la funcionalidad de creación de un objeto.

***
En su forma más simple (idiomática, no patrón), encapsular la creación de objetos es pasar de esto
![[Pasted image 20250203174832.png]]
a esto
![[Pasted image 20250203174927.png]]
![[Pasted image 20250203174951.png]]
de manera de instanciar una factory en PizzaStore y delegar la creación de cada Pizza a la Factory.
¿No es lo mismo, pero solo delegando la creación a otro objeto? No, porque puede haber múltiples clientes de la factory, y con este enfoque se [[Principio de Diseño 3 - Favorecer la composición a la herencia|encapsula lo que cambia]] para que, cuando lo haga, modificar solo una parte del código