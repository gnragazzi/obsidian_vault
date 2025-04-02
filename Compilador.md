Programa (o conjunto de programas) que traduce un lenguaje a otro.
Por ejemplo, traduce de un [[Lenguajes de Programación|Lenguaje]] de Alto Nivel a Lenguaje de Máquina.
***
La compilación tiene una fase de análisis, que está dividida en:
- [[Analizador Lexicográfico|Análisis Lexicográfico]] (*Scanner*)
	- Su objetivo es transformar la entrada para que pueda ser usada por el parser.
	- Es invocada por el Parser, recibiendo solicitud de *Deme Próximo Token*, luego leé los caracteres de entrada hasta que pueda delimitar un token y lo retorna.
	- También "limpia"  la entrada, eliminando comentarios, espacios en blanco, tabulaciónes, etc...
- [[Análisis Sintáctico]] (*Parser*).
	- Normalmente, implementa el Analizador Lexicográfico como una subrutina.
***
Razones para Separar el Ánalisis en 2:
1. Facilita el diseño de compiladores
2. Compilador es más eficiente
3. Compilador más portable (porque es el analizador lexicográfico el que se encarga de las palabras especiales).