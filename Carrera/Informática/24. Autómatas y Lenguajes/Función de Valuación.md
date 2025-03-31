La función $ϕ:L_{ER}→2^{Σ^*}\color{red}[1]$, es denominada la función de valuación.
$L_{ER}$ es el conjunto de todas las posibles [[Expresiones Regulares - Lenguajes|expresiones regulares]]. 
$ɸ$ toma como argumento una expresión regular bien formada [[Definición Recursiva de E.R.|según esta definición]] y da como resultado el conjunto de cadenas denotado por dicha expresión. Luego ^427c8a
- $ϕ(∅) = \{\}$ el conjunto vacío
- $ϕ(λ) = \{λ\}$ el conjunto formado por la [[Cadena - Lenguajes#^41d68b|cadena de longitud nula]].
- $ϕ(a) = \{a\}$ el conjunto formado por la cadena $a$.
- $ϕ(E.F) = ϕ(E).ϕ(F)$ el conjunto formado por la concatenación de conjuntos.
- $ϕ(E+F) = ϕ(E)∪ϕ(F)$ el conjunto formado por la concatenación de conjuntos.
- $ϕ(E*) = ϕ*(E)$ clausura de un conjunto
- $ϕ((E)) = ϕ(E)$ 
***
[1]. [[Conjunto de Partes#^d7cf39|Notación Alternativa para el conjunto de partes]] 