- La consulta se realizará como respuesta a la llamada de un método
- Idealmente, estas consultas se ubicarán en la capa Repository
- Consulta
	- Debe estar marcada arriba del método con la anotación `@Query(<consulta>)`.
	- En el caso de necesitar hacer uso de un parámetro en la consulta (pasado como parámetro al método, por ejemplo) se marca el nombre de dicho atributo anteponiendo `:`, de la siguiente manera:
		- `:<nombreParametro>`
- Método
	- Su tipo de retorno debe coincidir con lo que retorna la consulta
	- De haber parámetros, en la lista de parámetros se deben puntualizar usando la anotación:
		- `(@Param("<nombreParámetro") <tipo> <identificador>)` 
			- `<nombreParámetro>` debe coincidir en la consulta y en la lista de parámetros.
	- Nombrar siguiendo las [[Buenas prácticas de nombrado de métodos en consultas HQL]]  