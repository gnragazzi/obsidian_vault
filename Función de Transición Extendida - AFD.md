$δ^+:Q×Σ^*→Q$
Definición Recursiva de $δ^+:Q×Σ^*→Q$
1. $δ^+(q,λ)=q$
2. $δ^+(q,w)=δ(δ⁺(q,x),σ)$ con 
	1. $x∈Σ^*$
	2. $σ∈Σ$
	3. $w=xσ$
***
En consecuencia, una [[Cadena - Lenguajes|cadena]] $w$ es aceptada por un [[Autómata Finito Determinístico|AFD]] $M = (Q, Σ, δ, q_0 , F )$ si $$δ⁺(q_0,w)∈F$$
Y el [[Lenguaje - Definición|lenguaje]] aceptado por M puede ser definido en términos de la función de Transición Extendida$$L(M)=\{w∈Σ^*|δ⁺(q_0,w)∈F\}$$

***
![[Pasted image 20250323113223.png]]
El símbolo usado, un delta con acento agudo encima, no es posible con unicode, por eso, la alternativa $δ⁺$ 