***Coloquialmente***
- Un sistema formal es un conjunto de reglas que pueden ser aplicadas a cierta información inicial para derivar información adicional.
- Se emplean símbolos **cuyo comportamiento y propiedades están completamente determinados** por estas reglas (por lo tanto, no hay que asumirles propiedades!!).
***
**Formalmente**
1. Un **[[alfabeto]]** de [[Símbolo|símbolos]]. 
	1. El alfabeto de un sistema formal es el conjunto de símbolos que pertenecen al [[Lenguaje - Definición|lenguaje]] del sistema en el que se necesita trabajar.
2. Un conjunto de [[Cadena - Lenguajes|cadenas]] finitas de dichos símbolos, llamadas _fórmulas bien formadas (fbf)_. 
	- Una vez definido el alfabeto, se debe determinar qué combinaciones de símbolos pertenecen al lenguaje del sistema. Esto se logra mediante una [[gramática]] formal. Las cadenas de caracteres construidas según esta gramática son las _fórmulas bien formadas_.
3. Un conjunto de fórmulas bien formadas, llamadas _axiomas_. 
	- Los [[Axioma|axiomas]] de un sistema axiomático son un conjunto de _fbf_ que se asumen como verdaderas (si se realiza la tabla de verdad de las mismas se puede ver que son tautologías) y se toman como punto de partida para las demostraciones.
4. Un conjunto finito de _reglas de deducción_ (o de inferencia). 
	- Una regla de inferencia es una [[Función (Discretas)|función]] que asigna una fórmula (conclusión) a un conjunto de fórmulas (premisas). 
	- Naturalmente la idea es que las reglas de inferencia transmitan la verdad de las premisas a la conclusión, es decir que sea imposible alcanzar una conclusión falsa a partir de premisas verdaderas.
