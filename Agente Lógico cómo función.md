```
función Agente-BC(percepción) retorna una acción  
	static: BC, una base de conocimiento  
	        t, un contador, inicializado en 0, que indica el tiempo  
	Decir(BC, Crear-Sentencia-De-Percepción(percepción, t))  
	acción ← Preguntar(BC, Crear-Consulta-Acción(t))  
	Decir(BC, Crear-Sentencia-Acción(acción, t))  
	t ← t + 1  
	retornar acción
```
 [[Crear-Sentencia-Percepción]] 