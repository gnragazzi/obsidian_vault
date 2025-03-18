Sea $X ∈ A^∗$, una [[Cadena - Lenguajes|lista de símbolos]] de [[Alfabeto de la Lógica Proposicional|A]]. Llamaremos ***peso de X***, y lo denotaremos por $peso(X)$, al número entero que se obtiene restando al número de paréntesis izquierdos “(” el de paréntesis derechos “)” que figuran en la lista $X$.
***
$X$ es una lista cualquiera de símbolos de X y no necesariamente una [[Fórmula Lógica]]. ^4209c9

***
- Para toda [[Variables Proposicionales|variable proposicional]] $p_n$, $peso(p_n) = 0$  ^a0fe8c
- $peso(¬X) = peso(X)$  ^e005ac
- si ∗ denota uno cualquiera de los conectivos $∨, ∧,→$, entonces:  ^ebce42
	- $peso((X ∗ Y )) = peso(X) + peso(Y )$