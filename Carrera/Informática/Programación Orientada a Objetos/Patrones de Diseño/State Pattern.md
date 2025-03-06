*Permite a un objeto alterar su comportamiento cuando su estado interno cambia. El objeto va a aparentar cambiar de clase*.
***
La segunda parte de la definición hace referencia a la perspectiva del cliente: el comportamiento puede llegar a ser completamente distinto, lo cual asemeja a que el objeto cambio a otra clase que implementa la misma interfaz. Esto se logra a través de la [[Composición]].
***
![[Pasted image 20250306072831.png]]
***
Está muy relacionado con el [[Strategy Pattern]]: en resumen, son iguales en estructura, pero distintos en intención.
El Strategy permite configurar una serie de comportamientos que se determinan para la clase contexto, y que pueden cambiar en tiempo de ejecución, evitando el uso de la herencia y obteniendo así diseños más flexibles; mientras que el State Pattern determina una serie de comportamientos que varían según una serie finita y discreta de estados.
***
 Variantes:
 - La clase abstracta *State* puede implementar métodos comunes (por ejemplo, errores en ciertos comportamientos) para evitar repetición de código.
 - La lógica de transición (dónde se elige y aplica el cambio de estado) puede manejarse en los estados o en el contexto
	 - Cada opción tiene su pro y su contra
 - Si se tienen varios contextos, se pueden usar los mismos estados (siempre que estos estados no necesiten hacer un seguimiento de un estado interno).
	 - Por ejemplo, siendo variables estáticas dentro del contexto
***
Principios de Diseño utilizados.
- [[Principio de Diseño 1 - Encapsular lo que cambia]]
	- En este contexto, lo que cambia es el estado (como el *Context* actua según se dan distintas condiciones) y se encapsula creando clases para cada uno de los estados, y permitiendoles a estos manejar el comportamiento.
- [[Principio de Diseño 2 - Programar a la interfaz]]
	- Se programa desde *Context* pensando en la interfaz *State* y no en las implementaciones concretas.
- [[Principio de Diseño 4 - Bajo Acoplamiento]]
	- El *Cliente* no conoce como *Context* maneja su comportamiento (de hecho, sería un error que el cliente pueda determinar o forzar cambios de estado de manera directa), y *Context* no sabe de la implementación que hacen los estados concretos de *handle()*.
- [[Principio de Diseño 5 - abierto'cerrado]]
	- Los estados concretos están cerrados a la modificación, y si se quiere agregar un nuevo estado, se consigue extendiendo/implementando la clase_abstracta/interfaz.
- [[Principio de Diseño 6 - Principio de Inversión de Dependencias]]
	- Dentro de cada método en *Context* hay una llamada a métodos definidos en una abstracción y no una clase particular.
- [[Principio de Diseño 9 - Principio de la Responsabilidad Única]]
	- Se cumple en la medida que se defina una clase *ConcreteState* por cada estado: de esta manera cada estado tiene una única responsabilidad.