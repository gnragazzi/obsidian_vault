Define una [[Interfaz - OOP|interfaz]] para crear un objeto, pero deja que las subclases decidan que clase instanciar.
Deja que una clase delege la instanciación a subclases.
***
La superclase no sabe que objeto va a ser instanciado, se dice que la "*subclase decide*", lo que en realidad significa que la decisión se realiza cuando se elige un creador concreto.
***
![[Pasted image 20250203175706.png]]
Tenemos productos concretos (que son los componentes de [[Componentes de Bajo Nivel|bajo nivel]]) que implementan la misma interfaz (en el sentido de colección de métodos de la clase abstracta *Product*) y tenemos un *Creador* abstracto que define una operación `anOperation()` que hace uso del `factoryMethod()`, definido este último como método abstracto. Cada creador concreto extiende la clase abstracta obligado a redefinir el `factoryMethod()` creando un producto concreto y devolviendolo a la operación `anOperation` que lo invoca.
***
- [[Principio de Diseño 8 - Principio Hollywood]]
	- porque los componentes de bajo nivel implementan interfaces, de manera que la comunicación del cliente es con los de alto nivel y los de bajo nivel no necesitan comunicarse con sus superiores.
***
[Head first Design Patterns]