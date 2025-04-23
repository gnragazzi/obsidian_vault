La ***longitud modificada*** de una [[Fórmula Lógica|fórmula]] P, que denotamos con $$long*(P)$$se define como el [[Grado de Complejidad de una fórmula|grado de complejidad]] de $P$ más el número de variables que figuran en P, contadas tantas veces como aparezcan repetidas.
***
Es la función$$long*:Form\mapsto\mathbb{N}$$
caracterizada por las siguientes propiedades:
- $(LM_1)$ Para toda variable proposicional $p_n$, $long*(p_n)=1$
- $(LM_2)$ Para toda fórmula $P$, $long*(\neg P)=1 + long*(P)$ 
- $(LM_1)$ Para todo par de fórmulas $P$ y $Q$, $$long*(P\lor Q)=long*(P\land Q)=long*(P\rightarrow Q)=long*(P)+log*( Q)+1$$
***
[[Longitud de Cadena]]