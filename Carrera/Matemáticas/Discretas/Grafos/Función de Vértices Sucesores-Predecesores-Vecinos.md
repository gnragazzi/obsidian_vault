Sea $G=<X,U,γ>$ un [[Digrafo - Definición Formal|digrafo]]/[[Grafo - Definición Formal|grafo]]
- El conjunto de todos los ***vértices sucesores*** de un vértice $x∈X$ se obtiene con la función $$Γ⁺: X→2^X \text{tal que}$$$$Γ⁺(x)≝\{y:(∃u∈U)∧γ(u)=(x,y)\}$$
- El conjunto de todos los ***vértices predecesores*** de un vértice $x∈X$ se obtiene con la función $$Γ^-: X→2^X \text{tal que}$$$$Γ^-(x)≝\{y:(∃u∈U)∧γ(u)=(y,x)\}$$
- El conjunto de todos los ***vértices vecinos*** de un vértice $x∈X$ se obtiene con la función $$Γ≝Γ⁻∪Γ⁺$$