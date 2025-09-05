#### Definición
- Acción o serie de acciones que llevan adelante un usuario o programa de aplicación que lee y/o modifica el contenido de una BD.
- Una transacción es atómica y **siempre** finaliza
- Un SGBD que implementa transacciones, debe cumplir con los [[Principios ACID]]
***
#### ¿Qué representa?

> [! Una unidad lógica de procesamiento que debe completarse en su totalidad para garantizar su exactitud]

***
#### Formato de una Transacción

```
Inicio de la transacción T_x  <--- BD CONSISTENTE
	... Procesamiento ...     <--- BD posiblemente INCONSISTENTE
Fin de la transacción T_x     <--- BD CONSISTENTE
```

***
#### Estados finales
- Éxito:
	- Se notifica al SGBD que los cambios deben persistirsse
	- Las demás transacciones verán el resultado de esta transacción
	- Es un punto de no retorno
- Fallo
	- Indica al SGBD que no debe aplicar los cambios a la BD
	- Se retorna al estado anterior del inicio de la transacción

[[Estados de una Transacción]]
***
#### Etiquetas
- #falta 