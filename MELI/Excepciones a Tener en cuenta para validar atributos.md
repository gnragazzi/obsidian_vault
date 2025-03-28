![[Captura de pantalla 2025-03-26 a la(s) 3.30.53 p. m..png]]
Son 2:
- Method ArgumentNotValidException
	- El mensaje que le mandamos al definir la propiedad está en `ResponseEntity.status(400).body(e.getBindingResult().getAllErrors().getFirst().getDefaultMessage());`
- HttpMessageNotReadableException
	- No tengo muy claro bajo que circunstancias tira esta excepción.
