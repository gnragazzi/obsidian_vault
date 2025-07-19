```c
Entrada: Una GLC G = ⟨N, Σ, P, S⟩ noncontracting  
Salida: Una GLC G_C = ⟨N_C, Σ, P_C, S_C⟩ que satisface:  
  a. L(G_C) = L(G)  
  b. G_C no contiene producciones encadenadas  

1. Para todo A ∈ N construir el conjunto CHAIN(A) (ver Algoritmo 4)  
2. La producción A → w ∈ P_C si hay un no terminal B y una cadena w que satisface:  
    2.1 B ∈ CHAIN(A)  
    2.2 B → w ∈ P  
    2.3 w ∉ N
```
#v2 
