```pascal
Entrada: una GLC G = ⟨N, Σ, P, S⟩  
Salida: El conjunto de no terminales anulables de G, llamado NULL  

1. NULL := {A / A → λ ∈ P}  
2. repetir  
    2.1 PREV := NULL  
    2.2 Para cada no terminal A ∈ N  
        Si hay una producción A → w y w ∈ PREV* entonces  
            NULL := NULL ∪ {A}  
   hasta NULL = PREV
```
#v2 