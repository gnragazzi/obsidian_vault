- @JsonPropertyOrder
	- Se utiliza a nivel de clase para definir el orden de los atributos del Json
	- Se puede utilizar una lista de identificadores entre corchetes
		- `@JsonPropertyOrder(values= {"name","age"})`
		- También se puede usar ordenes preestablecidos (alfabético, por ejemplo).
- @JsonFormat
	- Sirve para establecer un formato para parsear un string de manera de poder convertirlo a un LocalDate!!!!
	- 
		```
		@JsonFormat(pattern = "dd-MM-yyyy")
		private LocalDate birthDay;
		```
	- Convertirá un string que sigue ese formato en un objeto localdate válido.
		

![[Captura de pantalla 2025-03-26 a la(s) 3.39.14 p. m..png]]