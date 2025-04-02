1. Se crea un programa `.lex`con la especificación para el [[Analizador Lexicográfico]] en [[JFlex]].
	1. Solo detalla acciones a realizar cuando se encuentra un token, sin detalles de cómo se detecta.
2. Se compila el .lex con el compilador JFlex
	1. retorna un `Xylex.java`
3. Se compila con Java, utilizando el Xylex.java
	1. ![[Pasted image 20250402125537.png]]
4. Se transforma un txt de entrada en una secuencia de tokens, usando el archivo .`java` compilado en 3.
***
![[Pasted image 20250402125451.png]]
