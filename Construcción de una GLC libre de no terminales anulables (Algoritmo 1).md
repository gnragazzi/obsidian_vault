```pascal
Dada una GLC G = ⟨N, Σ, P, S⟩  
Entrada: Una GLC G′ = ⟨N′, Σ, P′, S′⟩ donde  
    G′ = G si S no aparece en el lado derecho de ninguna producción  
    Caso contrario, se designa un nuevo símbolo inicial S′  
    Se incorpora una nueva producción S′ → S en P′ y  
    N′ = N ∪ {S′}

Salida: Una GLC G_L = ⟨N_L, Σ, P_L, S_L⟩ que satisface  
    a. L(G_L) = L(G)  
    b. S_L no aparece en el lado derecho de ninguna producción  
    c. A → λ ∈ P_L si y sólo si λ ∈ L(G) y A = S_L

1. Se construye el conjunto NULL de no terminales anulables (ver Algoritmo 2)  
2. N_L es igual a N′  
3. P_L se define como:  
    3.1. Si λ ∈ L(G′) entonces S_L → λ ∈ P_L  
    3.2. Si A → w ∈ P′, y w puede ser escrito como:  
         w₁A₁w₂A₂...w_kA_kw_{k+1} donde A₁,A₂,…,A_k son un subconjunto  
         de las ocurrencias de no terminales anulables en w, entonces  
         A → w₁w₂…w_kw_{k+1} es una producción de P_L  
         Si w contiene n no terminales anulables, se obtendrán 2ⁿ producciones  
         Por ejemplo, si A,B,C ∈ N, A,B ∈ NULL, a ∈ Σ y A → CABAa ∈ P′.  
         Luego en P_L se suman las siguientes producciones:  
            A → CABAa  
            A → CABa  
            A → CAa  
            A → Caa  
    3.3. Si A → w ∈ P′ y no cumple con el punto 3.2, luego A → w ∈ P_L  
    3.4. A → λ ∈ P_L sólo si λ ∈ L(G) y A = S_L (elimina toda producción nula)

```
#v2 