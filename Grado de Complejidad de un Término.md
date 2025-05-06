Llamaremos *grado de complejidad de un término t* con $t\in L_\sigma$ y lo denotaremos $comp(t)$, al número de símbolos de función que figuran en la expresión $t$, contados tantas veces como aparezcan.
Observemos que:
- $comp(t)=0$ si y sólo si $t$ es una [[Alfabeto de la Lógica de Primer Orden#^638c55|variable o una constante]],
- Si $t=f(t_1,...,t_k)$ donde $f$ es un símbolo de función $k$-aria y los $t_i$ son términos, entonces$$comp(t)=comp(t_1)+...+comp(t_k)+1$$
