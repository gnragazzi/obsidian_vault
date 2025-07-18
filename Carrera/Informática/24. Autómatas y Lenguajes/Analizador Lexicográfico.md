### Definición 

Parte de un [[Compilador]], cuya tarea es leer los caracteres de entrada (el código fuente) para generar, a partir de ellos, los [[Token|tokens]] que serán luego utilizados en el [[Análisis Sintáctico]]. 
Siempre reconoce el token que se corresponde con el [[Lexema|lexema]] más largo.

### Representación de Tokens

Cuando el *A.L.* aisla un token, envía al A.S. un código interno que lo identifica como respuesta; respuesta que, por lo general, se representa como un par *(código, valor)*:

![[Pasted image 20250402124322.png]]
Es importante tener en cuenta que el valor puede ser inexistente, esto divide las respuestas posibles en 2 categorías:
1. $(Código,valor)$: identificadores, constantes, rótulos, etc.  
2. $(Código,λ)$: palabras reservadas, operadores, signos, etc.

***
### Lugar en el compilador

![[Pasted image 20250718082129.png]]

*** 
### Implementación

- [[Diseño e Implementación de Analizadores Lexicográficos]] 
	- Existe un lenguaje llamado lex que es un lenguaje de acción por patrón Se pueden especificar patrones utilizando [[Expresiones Regulares - Lenguajes|E.R.]] y Lex las convierte en [[Autómatas Finitos]].  Nosotros, lo implementaremos con [[JFlex]]
- [[Detección de Errores en el Análisis Lexicográfico]] 

***
### Etiquetas
#v2 