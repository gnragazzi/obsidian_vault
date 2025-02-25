Se asegura que una clase tiene una sola instancia y provee un punto de acceso global a dicha instancia.
***
![[Pasted image 20250210094010.png]]
***
Logramos los objetivos del patrón:
- Manteniendo una variable estática y privada de la misma clase
- Haciendo el constructor privado
- Proveyendo un punto de acceso que es un método público y estático que devuelve una instancia de la clase
	- Una variable es que, en caso de que no exista dicha instancia, la cree. Esto mejora el rendimiento al asegurarnos que no se creará la variable si no se usa.
***
Este patrón puede funcionar raro al usarse en ambientes de multithreading.
En tal caso, se puede:
- Usar la palabra sincronized (empeora el rendimiento de getInstance)
- Instanciar la variable privada-estática en la declaración, en lugar de en getInstance()
- Declarar a la variable como "volatile".
[Head First Design Patterns]
***
También puede haber problemas para asegurar que singleton funcione bien debido al uso de distintos [[Java Class Loader]]s