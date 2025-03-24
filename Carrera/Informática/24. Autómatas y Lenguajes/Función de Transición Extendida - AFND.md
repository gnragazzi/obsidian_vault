$δ^+:Q×Σ^*→2^Q$
Definición Recursiva de $δ^+$
1. $δ^+(q,λ)=\{q\}$
2. $δ^+(q,w)=\{r_1,r_2,...,r_m\}$
	1. $w=xσ$,
	2. $δ^+(q,x)=\{p_1,p_2,...,p_k\}$ 
	3. $\bigcup\limits_{i=1}^{k} δ(p_i,σ)=\{r_1,r_2,...,r_m\}$

***
![[Pasted image 20250323192225.png]]

Si $M$ es un [[Autómata Finito No Determinístico|AFND]], luego $$L(M)=\{w∈Σ^*|δ⁺(q_0,w)∩F≠∅\}$$

***
![[Pasted image 20250323113223.png]]
El símbolo usado, un delta con acento agudo encima, no es posible con unicode, por eso, la alternativa $δ⁺$ 