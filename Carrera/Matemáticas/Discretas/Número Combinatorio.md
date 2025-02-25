El número de combinaciones que tenemos de $m$ elementos elegidos entre un conjunto de cardinalidad $n$
$${n\choose{m}}=\frac{n!}{m!(n-m)!}$$
***
- $0! = 1$
- ${n\choose{m}}=0$ si $m>n$
***
Relacionado con una [[Permutación r de n elementos]], vemos que es una selección **no ordenada** de m elementos entre n. Por lo que una permutación puede construirse:
1. Eligiendo una combinación de m entre n elementos,
2. [[Permutacion de n elementos|Ordenando]] de m! maneras por el [[Principio de la Multiplicación]]
De tal manera, $$P_m^n=m!{n\choose{m}}$$ por lo que $${n\choose{m}}=\frac{P_m^n}{m!}= \frac{n(n-1)(n-2)...(n-m+1)(n-m)(n-m-1)...(2)(1)}{(n-m)(n-m-1)...(2)(1).m!}=\frac{n!}{(n-m)!m!}$$
