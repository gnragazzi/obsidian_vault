#### Definición Formal
- $L_d=\{x_i\in\{0,1\}^* / x_i\notin L(MT_i)\}$

***
#### Demostración de que $L_d$ no es [[Recursivamente Enumerable]]
(o lo que es lo mismo, que no existe MT M tal que $L(M)=L_d$ )
(por contradicción)
1. Supongamos que $L_d=L(M)$ para alguna [[Máquina de Turing|MT]] M.
2. Como $L_d$ es un lenguaje sobre el alfabeto binario, $M$ debería estar en la [[Proceso para encontrar un Lenguaje no R.E.|lista exhaustiva de MTs que aceptan estos lenguajes]].
3. Por lo tanto, hay al menos una MT $M_i$ tal que $M=M_i$.
4. Ahora, nos preguntamos si $x_i$ (la $i$-ésima cadena, según el [[Orden Canónico]]), se encuentra en $L_d$
	1. Si $x_i\in L_d$ significa que $M$ (y por lo tanto $M_i$) acepta la $x_i$. Pero, por definición de $L_d$, si $x_i\in L(M_i)$ entonces $x_i\notin L_d$.
	2. Si $x_i\notin L_d$ significa que $M$ (y por lo tanto $M_i$) no acepta la $x_i$. Pero, por definición de $L_d$, si $x_i\notin L(M_i)$ entonces $x_i\in L_d$.
5. Esta contradicción (una cadena perteneciendo y no perteneciendo al mismo tiempo a un lenguaje) surge de la suposición de que M existe. Por lo tanto, no existe M tal que $L_d=L(M)$ y, por lo tanto, L_d no es un lenguaje recursivamente enumerable.

***
#### Etiquetas
- #falta 