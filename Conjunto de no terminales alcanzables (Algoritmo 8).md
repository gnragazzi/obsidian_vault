```c
Entrada: Una GLC G = ⟨N, Σ, P, S⟩  
Salida: El conjunto de no terminales alcanzables, REACH  
1. REACH := {S}  
2. PREV := ∅  
3. repetir  
  3.1 NEW := REACH - PREV  
  3.2 PREV := REACH  
  3.3 Para cada no terminal A ∈ NEW hacer  
    Para cada producción A → w hacer  
      agregar todos los no terminales en w a REACH  
hasta REACH = PREV

```

#v2 