```c
Entrada: Una GLC G = ⟨N, Σ, P, S⟩  
Salida: El conjunto de no terminales que derivan en cadenas de terminales, TERM  
1. TERM := {A / hay una producción A → w ∈ P con w ∈ Σ*}  
2. repetir  
  2.1 PREV := TERM  
  2.2 Para cada no terminal A ∈ N hacer  
    Si hay una producción A → w y w ∈ (PREV ∪ Σ)* entonces  
      TERM := TERM ∪ {A}  
hasta PREV = TERM
```


#v2 