Convierte la interfaz de una clase en la interfaz que un cliente espera. Adapter permite que clases que eran incompatibles debido a sus interfaces, puedan trabajar juntas.
***
![[Pasted image 20250213110346.png]]
***
![[Pasted image 20250213103528.png]]
Tanto el cliente como *lo adaptado* están desacoplados: ninguno sabe el uno del otro.
***
- [[Principio de Diseño 1 - Encapsular lo que cambia]] - 
	- Porque lo que cambia es el código que necesita el cliente para hacer uso de lo adaptado, y está encapsulado en el adaptador.
- [[Principio de Diseño 2 - Programar a la interfaz]]
	- Porque el cliente utiliza la interfaz que adaptador implementa, y usa esa interfaz (y no las clases concretas)
- [[Principio de Diseño 3 - Favorecer la composición a la herencia]]
	- Porque el adaptador compone a lo adaptado.
- [[Principio de Diseño 4 - Bajo Acoplamiento]]
	- Porque el cliente, que hace uso de lo adaptado, no sabe nada de este.
- [[Principio de Diseño 5 - abierto'cerrado]]
	- Porque de esta manera el programa (cliente) está cerrado a la modificación (no hay que crear nuevo código dentro del cliente para hacer uso de lo adaptado).
- [[Principio de Diseño 6 - Principio de Inversión de Dependencias]]
	- Tal vez porque no hay dependencias a clases concretas: 
		- El cliente depende de una interfaz
		- El adaptador depende de la interfaz que se quiere adaptar
- [[Principio de Diseño 8 - Principio Hollywood]]
	- Porque la comunicación la comienza el componente de AN, al llamar a *request()*