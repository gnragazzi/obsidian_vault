Para toda [[Fórmula Lógica|fórmula]] $P$ valen las siguientes propiedades:
- (i) $peso(P)=0\color{red}^{[1]}$  ^d49e20
- (ii) Si $P = X ∗ Y$ , donde $X, Y∈A^*\color{red}^{[2]}$ , $∗$ ∈ {∨, ∧,→}, $⇒ peso(X) > 0$. ^f496f4
***
[1]. [[Peso de una Cadena]] 
[2]. [[Alfabeto de la Lógica Proposicional]] [[Lenguaje Referencial]] 
***
Ejemplo: 
$$P = (((p0 ∨ p1) → ¬p3) ∧ (p0 → p5))$$
- $peso(P ) = 0$ 
- a la izquierda del conectivo $∨$ $peso(\{(((p0\})=3>0$ 
- lo mismo ocurre con el peso de la lista a la izquierda de →, peso((((p0 ∨ p1))= 2 > 0. 
***
Demostración
- (i). (i) $peso(P)=0$
	- Llamemos S al conjunto de todas las [[Cadena - Lenguajes|listas]] de $A^∗$ que tienen peso 0:  $$S = \{X ∈ A^∗/peso(X) = 0\}$$  Del [[Peso de una Cadena#^a0fe8c|aquí]] resulta que todas las variables proposicionales pertenecen a S, y de [[Peso de una Cadena#^e005ac|aquí]] y [[Peso de una Cadena#^ebce42|aquí]] se deduce que $S$ es [[Cerrado por los Conectivos]]. Luego por el [[Teorema 1]], debe ser $Form ⊆ S$, esto es, todas las fórmulas tienen peso cero, lo que prueba el enunciado (i).
- (ii) Si $P = X ∗ Y$ , donde $X, Y∈A^*$ , $∗$ ∈ {∨, ∧,→}, $⇒ peso(X) > 0$.
	- Llamemos $T$ al conjunto de todas las [fórmulas] $X$ tales que, a la izquierda de cualquiera de los símbolos $∨, ∧, →$ que figuren en $X$ hay un número mayor de paréntesis que abren “(” que de paréntesis que cierran “)”.  
		- Una fórmula $P$ pertenece al conjunto T $⇔$ si asumiendo que $P$ es de la forma $P = X ∗ Y$ , donde $X, Y ∈ A^∗$, se cumple que el peso $(X) > 0$. 
			- Es decir que cualquier fórmula que pertenece al conjunto $T$, en caso de que sea de la forma $X*Y$, cumple con esta propiedad.
		- Como en las [variables proposicionales] sólo figuran los símbolos $p$ y $|$, éstas pertenecen trivialmente al conjunto $T$. 
		- Sabiendo que las [variables proposicionales] pertenecen a $T$, si demostramos que $T$ es [[Cerrado por los Conectivos]], sabremos que todas las fórmulas están en $T$. [[Teorema 1#^935052|¿Por qué?]] 
			- [[Cerrado por los Conectivos#^9ace17|(C1)]]
				- Para probar que T es [cerrado por los conectivos], suponemos que $P ∈ T$ y que $¬P = X ∗ Y$ . 
				- Recordar que si bien $P$ es fórmula, también es una [[Cadena - Lenguajes|lista de símbolos]] de $A^∗$, por lo cual, tanto $X$ como $Y$ pueden verse como [listas] de $A^∗$. 
				- Esto último implica que  $∃Z ∈ A^∗$ tal que $X = ¬Z$,  y por lo tanto que $P = Z ∗ Y$ . Como $P ∈ T$ , debe ser $peso(Z) > 0$, y por [[Peso de una Cadena#^e005ac|(5)]] se tiene que también  $peso(X) > 0$. Luego $¬P ∈ S$ y $T$ satisface [[Cerrado por los Conectivos#^9ace17|(C1)]].
			- (C2)
				- Sean $P,Q∈T$  y sea $∗ ∈ \{∨, ∧ , →\}$ que figuran en la lista $(P∨Q)$. 
				- Si ∗ figura a la izquierda de ∨, 
					- entonces $∃ X, Y ∈A^∗$ tales que $P = X∗Y ∧ (P ∨ Q) = (X ∗ Y ∨ Q)$. 
					- Como $P ∈ T$, debe ser $peso(X) > 0$, y como $peso((X) = 1 + peso(X)$, resulta que la expresión a la izquierda de $∗$ en $(P ∨ Q)$ tiene peso mayor que cero.  
				- Si $∗$ coincide con $∨$, 
					- entonces a la izquierda de ∗ figura (P , y como por la parte [(i)], $peso(P ) = 0$, resulta que $peso((P ) = 1 > 0$.  
				- Finalmente supongamos que ∗ figure a la derecha de $∨$. 
					- Entonces $∃X,Y en A^∗$ tales que $Q = X ∗ Y$ , y $(P ∨ Q) = (P ∨ X ∗ Y )$. Como $Q ∈ T$ , debe ser $peso(X) > 0$, y se tiene que peso$((P ∨ X) = 1 + peso(P ) + peso(X) = 1 + peso(X) > 0$ (dado que peso$(P) = 0$, por ser P fórmula).
					- Acabamos de ver así que la expresión a la izquierda de cualquiera de los símbolos $∨, ∧, →$ que figuran en la lista $(P ∨ Q)$, tiene siempre peso mayor que cero, lo que significa que $(P ∨ Q) ∈ T$ .  En forma enteramente análoga se prueba que si P y Q pertenecen a T , entonces también $(P ∧ Q) \text{ y } (P → Q)$ pertenecen al conjunto $T$ . Luego $T$ es [cerrado por los conectivos].  
					- Como $T$ es un subconjunto de $A^∗$ que contiene todas las [variables proposicionales] y es [cerrado por los conectivos], se cumple que Form ⊆ T : es decir todas las fórmulas satisfacen [(ii)], la condición que define al conjunto T , c.q.d.