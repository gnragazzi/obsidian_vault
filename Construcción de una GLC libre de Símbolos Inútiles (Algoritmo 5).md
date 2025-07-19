```c
Entrada: Una GLC G = ⟨N, Σ, P, S⟩  
Salida: Una GLC GU = ⟨NU, ΣU, PU, S⟩ que satisface:  
  a. L(GU) = L(G)  
  b. GU no contiene símbolos inútiles  
1. Construir la GLC GT donde todos los no terminales derivan cadenas de terminales, a través del Algoritmo 6  
2. Aplicar a GT el Algoritmo 8 para construir el conjunto de no terminales alcanzables  
3. NU = REACH  
4. PU = {A → w | A → w ∈ PT, A ∈ REACH, y w ∈ (REACH ∪ Σ)*}  
5. ΣU = {a ∈ Σ | a ocurre en el lado derecho de alguna producción PU}
```
#v2 
