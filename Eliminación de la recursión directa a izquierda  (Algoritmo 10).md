```c
Para remover la recursión directa a izquierda, las producciones se dividen en dos categorías:  
A. Las producciones directamente recursivas  
   A → Au₁ | Au₂ | ... | Auⱼ  
B. Las producciones:  
   A → v₁ | v₂ | ... | vₖ en las cuales el primer símbolo de vᵢ no es A  

Entonces para eliminar la recursión se agregan las siguientes producciones  
eliminando las producciones de las categorías A y B:  

  A → v₁Z | v₂Z | ... | vₖZ  
  Z → u₁Z | u₂Z | ... | uⱼZ | u₁ | u₂ | ... | uⱼ  
```

#v2 