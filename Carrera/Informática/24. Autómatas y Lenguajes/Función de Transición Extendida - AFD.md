$\hat{δ}+:Q×Σ^*→Q$
Definición Recursiva de $\hatδ:Q×Σ^*→Q$
1. $\hatδ(q,λ)=q$
2. $\hatδ(q,w)=δ(\hatδ(q,x),σ)$ con 
	1. $x∈Σ^*$
	2. $σ∈Σ$
	3. $w=xσ$
***
En consecuencia, una [[Cadena - Lenguajes|cadena]] $w$ es aceptada por un [[Autómata Finito Determinístico|AFD]] $M = (Q, Σ, δ, q_0 , F )$ si $$\hatδ(q_0,w)∈F$$
Y el [[Lenguaje - Definición|lenguaje]] aceptado por M puede ser definido en términos de la función de Transición Extendida$$L(M)=\{w∈Σ^*|\hatδ(q_0,w)∈F\}$$
