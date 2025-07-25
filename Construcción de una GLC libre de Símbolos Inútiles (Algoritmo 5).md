
>Entrada: Una $GLC$ $G = ⟨N, Σ, P, S⟩$  
   Salida: Una $GLC$ $G_U = ⟨N_U, Σ_U, P_U, S⟩$ que satisface:  
	a. $L(G_U) = L(G)$  
	b. $G_U$ no contiene símbolos inútiles  

1. Construir la $GLC$ $G_T$ donde todos los no terminales derivan cadenas de terminales, a través del [[Construcción de una GLC donde todo no terminal deriva cadenas de terminales (Algoritmo 6)|Algoritmo 6]]  
2. Aplicar a $G_T$ el [[Conjunto de no terminales alcanzables (Algoritmo 8)|Algoritmo 8]] para construir el conjunto de no terminales alcanzables  
3. $N_U = REACH$  
4. $P_U$ = $\{A → w \space|\space A → w ∈ P_T, A ∈ N_U, \text{ y } w ∈ (N_U ∪ Σ)*\}$  
5. $Σ_U = \{a ∈ Σ\space|\space \text{ a ocurre en el lado derecho de alguna producción } P_U\}$

***
#v2 
