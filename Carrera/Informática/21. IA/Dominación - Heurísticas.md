Sean $h_1$ y $h_2$ dos funciones [[Función Heurística - h(n)|heurísticas]] [[Admisibilidad|admisibles]]. Si $$∀n∈\text{Nodos}: h_2≥h_1$$ entonces se dice que $h_2$ ***domina*** a $h_1$.
***
Si una heurística domina a otra, es mejor para la búsqueda poque [[Búsqueda A*#^efd71a|nunca expandira más nodos]].
***
Dadas heurísticas admisibles $h_a$, $h_b$,  $h(n) = \max(h_a(n), h_b(n))$  es también admisible y domina a $h_a$ y $h_b$.
***