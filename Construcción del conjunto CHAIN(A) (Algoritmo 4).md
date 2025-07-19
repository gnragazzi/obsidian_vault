```c
Entrada: Una GLC noncontracting G = ⟨N, Σ, P, S⟩  
Salida: El conjunto de no terminales encadenados para el no terminal A, CHAIN(A)  

1. CHAIN(A) := {A}  
2. PREV := ∅  
3. repetir  
  3.1 NEW := CHAIN(A) − PREV  
  3.2 PREV := CHAIN(A)  
  3.2 Para cada no terminal B ∈ NEW hacer  
      Para cada producción B → C hacer  
        CHAIN(A) := CHAIN(A) ∪ {C}  
hasta CHAIN(A) = PREV

```

#v2 