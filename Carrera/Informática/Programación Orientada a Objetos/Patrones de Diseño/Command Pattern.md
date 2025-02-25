Encapsula un requerimiento como un objeto, dejandote parametrizar otros objetos con diferentes requerimientos, búsquedas, logs y soportar deshacer operaciones.
***
Básicamente es un objeto que evuelve otro objeto y una funcionalidad y da un único punto de acceso, llamado `execute()`
![[Pasted image 20250211124535.png]]
***
![[Pasted image 20250211124608.png]]
***
![[Pasted image 20250211124445.png]]
***
Este patrón puede ser usado para generar una cola de procesos que un pool de threads lleva a cabo 
[Head First Dessign Patterns - 230]
***
Este patrón también puede ser usado, junto con la [[Serialización de Objetos]] para guardar una secuencia de cambios en disco, de manera de recuperar esa secuencia de cambios en el caso de que el sistema se caiga. Esto puede usarse para [[Operaciones Transaccionales]]
![[Pasted image 20250212202513.png]]
