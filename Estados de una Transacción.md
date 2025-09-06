#### Estados
- Activa
	- Estado inicial
	- La transacción está en ejecución (operaciones de lectura/escritura).
- Parcialmente confirmada
	- Se han finalizado las operaciones
	- Los cambios están en memoria principal y aun no se han persistido
- Fallo
	- Ha ocurrido algún problema y los cambios deben ser desechos
- Confirmada
	- Los cambios realizados deben persistirse en la BD
***
#### Diagrama
![[Pasted image 20250905122856.png]]
***
#### Acciones de SGBD
- BEGIN (inicio de transacción)
- COMMIT (Confirmar)
- ROLLBACK (Abortar)
- Savepoints (puntos intermedios de recuperación)

***
#### Etiquetas
- #Anki 