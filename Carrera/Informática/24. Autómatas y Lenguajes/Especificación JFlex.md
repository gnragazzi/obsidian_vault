Consta de 3 partes
- Código de usuario
	- Fragmento de código copiado directamente en el archivo Xylex.
- Opciones y declaraciones
	- Declaraciones$$\matrix{
D_1=P_1\\
D_2=P_2\\
.\\
.\\
.\\
	D_n=P_n\\}$$
		donde $∀i≠j:D_i≠D_j$ y $P_i$ es una [[Expresiones Regulares - Lenguajes|E.R.]] construida a partir de $Σ∪\{D_1,...,D_{i-1}\}$ 
	- Opciones
		- `%class "nombre_clase"`  Crea la clase nombre_clase y genera el archivo nombre_clase.java en lugar de la clase Yylex en el archivo Yylex.java  
		- `%{ ... %}`  El fragmento de código delimitado por `%{` y `}%` es copiado a la clase generada por [[JFlex]] y es el lugar apropiado para definir la variables y funciones miembro.  
		- `%char`  Define la variable miembro `int yychar` la cual es un contador del número de caracteres (inicia en 0) leídos desde el comienzo del procesamiento de la entrada hasta el comienzo del token actual. 
		- `%line`  Define la variable miembro `int yyline` la cual es un contador del número de líneas (inicia en 0) leídas desde el comienzo del procesamiento de la entrada hasta el comienzo del token actual.  
		- `%column`  Define la variable miembro int yycolumn la cual es un contador del número de caracteres (inicia en 0) leídos desde el comienzo del procesamiento de la línea actual y hasta el comienzo del token actual.  
		- `%cup`  Esta opción habilita la compatibilidad con el Generador de Parser LALR para JAVA llamado `cup`  
		- `%full`  Esta opción genera el analizador compatible con una entrada con el conjunto de caracteres de 8 bits
		- `%unicode`  Esta opción genera el analizador compatible con una entrada con el conjunto de caracteres de 16 bits
	- Reglas Léxicas
		- Conjunto de [[Expresiones Regulares - Lenguajes|E.R.]] y acciones construidas como $$\matrix{
R_1\ \{acción_1\}\\
R_2\ \{acción_2\}\\
.\\
.\\
.\\
	R_m\ \{acción_m\}\\}$$donde 
			- $R_i∈Σ\{D_1,...,D_n\}$ y es una E.R. llamada [[Patrón - Análisis Lexicográfico|Patrón]]
			- $\{acción\}$ es un bloque de instrucciones Java que se ejecuta cuando una secuencia de [[Símbolo|símbolos]] matchea con $R_i$
				- La *acción* puede ser vacía
		- Se pueden hacer uso de métodos auxiliares, definidos a continuación:
		- `String yytext()`
			- Retorna la secuencia de caracteres que ha unificado con un patrón. 
		- `int yylength()` 
			- Retorna la longitud de la secuencia de caracteres que ha unificado con un patrón.
		- `int yyline` 
			- Variable que contiene el número de línea leídas desde el comienzo del procesamiento de la entrada. 
		- `int yychar`
			- Variable que contiene el número de caracteres leídos desde comienzo del procesamiento de la entrada.
		- `int yycolumn` 
			- Variable que contiene el número de caracteres leídos desde comienzo del procesamiento de la línea actual.
	
#v2 