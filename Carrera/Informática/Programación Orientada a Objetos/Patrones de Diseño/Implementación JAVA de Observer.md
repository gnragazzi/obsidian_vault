![[Pasted image 20250114100759.png]]
***
- La clase abstracta `Observable` para el subject
	- Tiene métodos (setChanged, notifyObserver, etc...)
	- hay que ejecutar setChanged antes de notificar (sino se ignora la notificación)
	- El orden de notificación es arbitrario.
- Interfaz `Observer`, implementada por el observador
- El hecho de que Observable sea una clase, limita el reuso porque no hay multiple herencia en Java. ( de esta manera, una clase que vaya a ser subject, no puede heredar de otros lados).
- Este tipo de implementación permite pull y push.
***
[[Java]]