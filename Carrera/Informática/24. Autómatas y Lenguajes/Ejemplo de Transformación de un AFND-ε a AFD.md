Se puede resumir el proceso en los siguientes pasos:
1. Determinar el estado inicial de $q_D$ haciendo la clausura de $q_0$.
2. $S←q_D$ 
3. $P←∅$  (procesados)
4. $R←∅$ (Restantes)
5. Mientras S no sea vacío 
	1. Para cada símbolo $σ∈Σ$ 
		1. siendo $S=\{p_1,...,p_k\}$
		2. $δ_D(S,σ)=\text{clausura-}ε(\bigcup_{i=1}^kδ_E(p_i,σ))$ 
		3. Si $\text{clausura-}ε(\bigcup_{i=1}^kδ_E(p_i,σ))∉R$ ni a $P$  
			1. $R.push(\text{clausura-}ε(\bigcup_{i=1}^kδ_E(p_i,σ)))$
	2. $P.push(S)$
	3. $S←R.pop()$
Al finalizar, $P=Q_D$.
***
![[Pasted image 20250404082742.png]]
![[Pasted image 20250404082754.png]]
![[Pasted image 20250404082805.png]]