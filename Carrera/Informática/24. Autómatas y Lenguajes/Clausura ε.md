Informalmente, ε-cerramos un estado $q$ si seguimos todas las transiciones desde $q$ que están etiquetadas como ε.
Formalmente, se define recursivamente:
1. El estado $q∈\text{clausura}-ε(q)$ 
2. Si $δ$ es la [[AFND-ε#^6f29e5|función de transición]] del [[AFND-ε]] y $p∈\text{clausura-}ε(q)$, entonces $\text{clausura-}ε(q)$ también contiene todos los estados en $δ(p,ε)$.