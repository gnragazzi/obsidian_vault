Una [[Función Heurística - h(n)|heurística]] es ***consistente*** si para cada nodo $n$ y cada sucesor $n'$ de $n$ generado  por la acción $a$, el costo estimado de llegar al objetivo desde $n$ no es mayor que el costo del paso de llegar a $n'$ más el costo estimado de llegar al objetivo desde  $n'$. En símbolos  $$h(n) ≤ c(n, a, n') + h(n')$$
***
![[Pasted image 20250329182801.png]]