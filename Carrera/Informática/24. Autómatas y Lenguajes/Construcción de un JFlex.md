1. Comienza a leer de a un caracter hasta que encuentra el prefijo más largo que unifica con algún $R_i$ 
	1. Si matchea con varias [[Expresiones Regulares - Lenguajes|E.R.]] elije la del $i$ menor
		1. Por lo que, palabras clave deben ser listadas ANTES que identificadores.
2. Lo almacena en el buffer, accesible desde [[yytext()]]
3. Ejecuta la acción $i$
4. Si en la acción $i$ hay un retorno, retorna el control.
	1. De otra manera, continua desde el paso 1.