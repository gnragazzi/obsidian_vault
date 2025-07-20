
Dada una GLC G = ⟨N, Σ, P, S⟩  
### Entrada: 
Una $GLC$ $G' = ⟨N', Σ, P', S'⟩$ donde  
- $G' = G$ si $S$ no aparece en el lado derecho de ninguna producción  
- Caso contrario, se designa un nuevo símbolo inicial $S'$  
- Se incorpora una nueva producción $S' → S$ en $P'$ y  
- $N' = N ∪ \{S'\}$

Salida: Una $GLC G_L = ⟨N_L, Σ, P_L, S_L⟩$ que satisface  
    a. $L(G_L) = L(G)$
    b. $S_L$ no aparece en el lado derecho de ninguna producción  
    c. $A → λ ∈ P_L$ si y sólo si $λ ∈ L(G) \land A = S_L$

1. Se construye el conjunto $NULL$ de no terminales anulables (ver [[Construcción del conjunto de no terminales anulables(Algoritmo 2)|Algoritmo 2]])  
2. $N_L$ es igual a $N'$
3. $P_L$ se define como:  
    1. Si $λ ∈ L(G')$ entonces $S_L → λ ∈ P_L$
	2. Si $A → w ∈ P'$, y $w$ puede ser escrito como: 
		1. $w_1A_1w_2A_2...w_KA_kw_{k+1}$ donde $A_1,A_2,…,A_k$ son un subconjunto de las ocurrencias de no terminales anulables en $w$, entonces $A → w_1w_2…w_kw_{k+1}$ es una producción de $P_L$.
		2. Si $w$ contiene $n$ no terminales anulables, se obtendrán $2^n$ producciones.
		3. Por ejemplo, si $A,B,C ∈ N$, $A,B ∈ NULL$, $a ∈ Σ$ y $A → CABAa ∈ P'$. Luego en $P_L$ se suman las siguientes producciones:           
            1. $A → CABAa$  
            2. $A → CABa$
            3. $A → CAa$  
            4. $A → Caa$  
    3. Si $A → w ∈ P'$ y no cumple con el punto 3.2, luego $A → w ∈ P_L$
    4. $A → λ ∈ P_L$ sólo si $λ ∈ L(G)$ y $A = S_L$ (elimina toda producción nula)

#v2 