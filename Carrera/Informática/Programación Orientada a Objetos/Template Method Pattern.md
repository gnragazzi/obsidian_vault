Define el esqueleto de un algoritmo en un método, delegando algunos pasos del algoritmo a subclases.
Deja que las subclases re-definan ciertos pasos del algoritmo sin cambiar la estructura del algoritmo.
***
![[Pasted image 20250214082805.png]]
***
Este patrón está muy relacionado con:
- [[Strategy Pattern]]
	- Porque ambos hablan de encapsular comportamiento. La diferencia es que SP lo hace componiendo esos comportamientos en interfaces que se pueden extender, mientras que TMP establece una estructura y cada sub-clase es la responsable de implementar las pequeñas diferencias.
- [[Factory Method]]
	- En este caso, la diferencia es la intención: FM se encarga de la creación de un objeto, y lo hace siguiendo la misma estructura general de TMP: delegar a una subclase ciertos pasos de un algoritmo.
***
En este método, hay un algoritmo (templateMethod en AbstractClass) compuesto enteramente por llamadas a otros métodos (primiteOperation en el diagrama) , algunos de ellos implementados (*concreteOperation*, los pasos de los cuales son comunes a todas las subclases (y deberían ser ***final***)) y otros *abstractos*, de manera que la forma particular en que cada sub-clase se encarga de esos pasos depende de la implementación que hagan las mismas al redefinir estos métodos.
Por último, hay una 3er clase de métodos, llamados *hooks*, para los cuales la clase abstracta define una implementación (o tal vez no lo hace) pero se deja la puerta abierta (al no implementar el método como final) para que las clases concretas re-definan el método, de manera de tener una capacidad de agregar alguna característica particular a la ejecución del algoritmo en algún punto
![[Pasted image 20250214083949.png]]
***
- [[Principio de Diseño 1 - Encapsular lo que cambia]]
	- Tal vez, pues es al revés: encapsula lo que se mantiene igual y lo que cambia se implementa en nuevas clases, de manera de que si necesito una versión diferente del algoritmo implementado en el TemplateMethod, solo dejo instanciar la clase abstracta.
- [[Principio de Diseño 2 - Programar a la interfaz]]
	- Porque el cliente de la clase abstracta definirá esta e instanciara una subclase.
- [[Principio de Diseño 6 - Principio de Inversión de Dependencias]]
	- Porque las clases de este patrón dependen únicamente de la clase abstracta
- [[Principio de Diseño 8 - Principio Hollywood]]
	- Hace uso de este principio de diseño porque es la super-clase abstracta la que inicia la comunicación con la sub-clase (el cliente de estas clases no definiría la variable como la clase concreta, sino como la abstracta e instanciaría la concreta). De esta manera, no hay dependencias hacia las subclases y estas solo se comunican con un componente de alto nivel (su super-clase) una vez que son llamadas (digamos, llaman al templateMethod o otras operaciones concretas definidas en la super clase).
