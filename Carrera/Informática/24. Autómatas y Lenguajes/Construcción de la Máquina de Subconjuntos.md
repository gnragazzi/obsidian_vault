### Definición
La construcción del subconjunto comienza a partir de un [[Autómata Finito No Determinístico|AFND]] $N = (Q_N, Σ, δ_N, q_0 , F_N )$. El objetivo es construir un [[Autómata Finito Determinístico|AFD]] $D = (Q_D, Σ, δ_D, {q_0} , F_D )$ tal que $$L(D)=L(N)$$
- $Q_D$ es el [[Conjunto de Partes|conjunto de partes o conjunto potencia]] de $Q_N$.
	- No significa que todos los estados son útiles (pueden ser descartados los que no sean accesibles desde $q_0$)
- $F_D =\{S⊆Q_n:S∩F_N≠∅\}$
- $∀ S⊆Q_N,∀a∈Σ:δ_D(S,a)=\bigcup_{p∈S}δ_N(p,a)$ 
***
### Teoremas
[[Teorema 1 - Equivalencia AFD - AFND]]
[[Teorema 2 - Equivalencia AFD - AFND]]

### Etiquetas

#v2 