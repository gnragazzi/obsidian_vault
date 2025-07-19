```c
Entrada: Una GLC G = ⟨N, Σ, P, S⟩ que cumple con:  
a. El símbolo de inicio de G es no recursivo  
b. G no contiene producciones λ, excepto S → λ  
c. G está libre de producciones encadenadas  
d. G está libre de símbolos inútiles  
Salida: Una GLC G′ = ⟨N′, Σ, P′, S⟩ que cumple con la definición de la FNC.  

1. Sea A → w una producción en P con |w| > 1, entonces remover los  
terminales del lado derecho de tales producciones, de la siguiente manera:  
  A → bDcF  
puede ser reemplazada por las siguientes producciones:  
  A → B′DC′F  
  B′ → b  
  C′ → c  

2. Se reemplaza la producción A por las siguientes producciones:  
  A → B′T₁  
  T₁ → DC′T₂  
  T₂ → CF  

3. Las restantes producciones de P que cumplen con la definición  
de la Forma Normal de Chomsky quedan en P′  
```
#v2 