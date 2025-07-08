La operación de concatenación ($.$), es una [[Relación Binaria|operación binaria]] entre [[Cadena - Lenguajes|cadenas]] de $Σ^∗$ , es decir:  
$$. : Σ^∗ × Σ^∗ → Σ^∗  $$
Dados $s,t\in A^*$,  indicaremos con $s.t$ (o $st$) a la lista de elementos de $A$ que se obtiene escribiendo la lista $t$ a continuación de la lista $s$.

Observación: 
- la [[Cadena - Lenguajes#^bb350b|***cadena vacı́a***]] $λ$ es el elemento ***neutro*** de la operación de concatenación:  
$$∀x ∈ Σ^∗: λx = xλ = x$$
- El conjunto vacío $∅$ es el ***absorvente*** de la concatenación$$∀x ∈ Σ^∗:x.∅=∅.x=∅$$
[Análisis Comparativo de Lenguaje - U3 Aspectos Formales del Diseño de Lenguajes]
[Lógica Para Computación U1]
***
$long(st) = long(s) + long(t)$
[[Longitud de Cadena]]
***
### Etiquetas
#v2 