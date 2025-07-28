
> Entrada: Una $GLC\space G = ⟨N, Σ, P, S⟩$  
   Salida: Una $GLC\space GT = ⟨N_T, Σ_T, P_T, S⟩$ que satisface:  
	  a. $L(G_T) = L(G)$  
	  b. Todo no terminal en $G_T$ deriva una cadena de terminales en $G_T$  

1. Construir el conjunto $TERM$ de no terminales que derivan en cadenas de terminales ( [[Construcción del conjunto de no terminales que derivan en  cadenas de terminales (Algoritmo 7)|Algoritmo 7]])  
2. $N_T = TERM$
3. $P_T = \{A → w\space |\space A → w ∈ P, A ∈ N_T, y w ∈ (N_T ∪ Σ)^*\}$  
4. $Σ_T = \{a ∈ Σ\space |\space \text{ a ocurre en el lado derecho de alguna producción en }P_T\}$
***
#v2 