$$δ:Q×(Σ∪{\lambda})×Γ→2^{Q×Γ^∗}$$
Es decir que la función de transición recibe una triupla. Está definida de la siguiente manera$$\delta(q, a, Z) = \{(p_1, \gamma_1), (p_2, \gamma_2), \ldots, (p_n, \gamma_n)\}$$donde, para $i=1..n$:
- $q_i∈Q$
- $\gamma_i\in \Gamma^*$

En toda transición, se tiene que: 
- Si $\gamma=\lambda$ entonces se hace ***pop*** en la pila
- Si $\gamma=X$ la pila no se modifica
- Si $\gamma=YZ$, $X$ es reemplazado por $Z$ e $Y$ es puesto en la pila.
	- Con $Y\in\Gamma^*,Z\in\Gamma$  
***
#v2 