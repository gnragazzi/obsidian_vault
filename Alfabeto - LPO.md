Se divide en:
- ##### Símbolos Lógicos ^638c55
	- variables 
		- $x_0,x_1,...$
	- Conectivos proposicionales
		- $∧,∨,¬,→$
	- Cuantificadores
		- $\forall$ cuantificador universal
		- $\exists$ cuantificador existencial
	- Símbolos auxiliares
		- $,$
- ##### Símbolos No Lógicos ^5a28ac
	- Una familia $\mathcal{F}$, de _símbolos de funciones_ $(f_i)_{i \in I}$ tal que para cada $f_i$ se tiene definida su aridad $n(i) \in \mathbb{N}$. Puede ser $I = \varnothing$, es decir que $\mathcal{F} = \varnothing$.
    - Una familia $\mathcal{P}$ de _símbolos de predicados_ $(P_j)_{j \in J}$ tal que para cada $P_j$ se tiene definida su aridad $m(j) \in \mathbb{N}$. Se exige que $J \ne \varnothing$, es decir que $\mathcal{P} \ne \varnothing$, esto es, que _haya al menos un símbolo de predicado_.
    - Una familia $\mathcal{C}$ de _símbolos de constantes_ $(c_k)_{k \in K}$. Puede ser que $K = \varnothing$, o sea 
***
- Si la aridad es igual a 1 se dice que la (función, predicado) es monádica. Caso contrario, se dice poliádica.
- Los símbolos lógicos son comunes a todos los lenguajes de primer orden, mientras que los símbolos de funciones, de predicados y de constantes forman el ***vocabulario*** de un lenguaje de primer orden y son particulares de cada lenguaje.
- Un lenguaje de primer orden queda determinado por su vocabulario, que simbolizaremos con$$\sigma = \left\langle (f_i)_{i \in I},\ (P_j)_{j \in J},\ (c_k)_{k \in K} \right\rangle$$
- El lenguaje construido a partir de este alfabeto lo denotamos $L_\sigma$
