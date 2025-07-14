
### Definición Formal

Sea $E=(Q_E,Σ,δ_E,q_0,F_E)$ un [[AFND-ε]]. Entonces, el [[Autómata Finito Determinístico]] equivalente es$$D=(Q_D,Σ,δ_D,q_D,F_D)$$definido como:
1. $Q_D$ es el [[Conjunto de Partes]] de $Q_E$.
	- Se encuentra que todos los estados accesibles de $D$ son conjuntos ε-clausurados de $Q_E$, esto significa conjuntos $S⊆Q_E$ tal que $S=\text{clausura-}ε(S)$.
2. $q_D=\text{clausura-}ε(q_0)$.
3. $F_D=\{S|S⊆Q_D∧S∩F_E≠∅\}$
4. $δ_D(S,a)$ es computado, para $∀a∈Σ,S⊆Q_D$ como:
	- (a) $S={p_1,...,p_k}$
	- (b) $\bigcup_{i=1}^kδ_E(p_i,a)=\{r_1,r_2,...,r_m\}$ 
	- $(c) δ_D(S,a)=\text{clausura-}ε(\{r_1,r_2,...,r_m\})$ 
***
[[Ejemplo de Transformación de un AFND-ε a AFD]] 
[[Teorema 2.22 - Sobre la equivalencia de AFD y AFND-ε]] 

***
### Etiquetas

#v2 