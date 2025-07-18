### ¿Qué implica programar un A.L.?

Especificar y deseñar un programa que ejecute acciones guiadas por los [[Patrón - Análisis Lexicográfico|patrones]] que aparecen en las [[Cadena - Lenguajes|cadenas]]. 
### ¿Con qué se necesita contar?

Se necesita contar con:
1. Método para Describir [[Patrón - Análisis Lexicográfico|patrones]] que se asocien con [[Token|tokens]].
	1. [[Expresiones Regulares - Lenguajes]]
2. Mecanismo reconocedor de Tokens
	1. [[Autómatas Finitos]]
3. Agregar acciones al Autómata Finito
	1. De esto surge un [[Autómata Finito con Acciones Semánticas]]. 
	2. ![[Pasted image 20250402124641.png]]

***
### ¿Cuál es el proceso del A.L.?

1. Delimitar [[Lexema]]
2. Asignar el código de Token que corresponda.
Estrategias:
***
### ¿Cuál es la estratégica utilizada por un A.L.?

- Palabras clave
	- Reservadas
		- Eliminar como camino alternativo y tratar como identificadores.
		- Se tiene una tabla donde cada vez que se delimita un identficador observa si es una palabra clave (en este caso, devuelve $(código,λ$)).
		- Si no, verifica la tabla de símbolos
			- Si no está lo agrega
			- De todas fórmas devuelve el código de `identificador` y el valor
	- No reservadas
		- Agregando al autómata contexto (transiciones que reconozcan estas palabras clave)
- Espacios en blanco, tabls, newline, etc
	- Significativos
		- Blancos entre tokens que son tomados como delimitadores/separadores
	- No significativos
		- Se borran y delimita con otros símbolos
***
#v2 