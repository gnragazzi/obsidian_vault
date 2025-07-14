### Definición Informal

> ε-cerramos un estado $q$ si seguimos todas las transiciones desde $q$ que están etiquetadas como ε.

### Definción Formal

Sea q un estado de un $AFND-ε$. Definimos formalmente de manera recursiva la $clausura-\epsilon$ para $q$, como:
1. El estado $q∈\text{clausura}-ε(q)$ 
2. Si $δ$ es la [[AFND-ε#^6f29e5|función de transición]] del [[AFND-ε]] y $p∈\text{clausura-}ε(q)$, entonces $\text{clausura-}ε(q)$ también contiene todos los estados en $δ(p,ε)$.

### Etiquetas
#v2 