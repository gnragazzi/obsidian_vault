```c
Entrada: Una GLC G = ⟨N, Σ, P, S⟩  
Salida: Una GLC GT = ⟨NT, ΣT, PT, S⟩ que satisface:  
  a. L(GT) = L(G)  
  b. Todo no terminal en GT deriva una cadena de terminales en GT  
1. Construir el conjunto TERM de no terminales que derivan en cadenas de terminales (ver Algoritmo 7)  
2. NT = TERM  
3. PT = {A → w | A → w ∈ P, A ∈ TERM, y w ∈ (TERM ∪ Σ)*}  
4. ΣT = {a ∈ Σ | a ocurre en el lado derecho de alguna producción en PT}
```

#v2 