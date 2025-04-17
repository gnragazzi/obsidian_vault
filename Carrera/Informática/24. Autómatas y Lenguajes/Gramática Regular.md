Una gramática regular es una 4-upla $(V,Σ,R,S)$ en donde:
- $V$ es un [[Alfabeto]]
- $Σ⊆V$ que contiene a los [[Reglas Gramaticales#^6fb4ac|símbolos terminales]]
- $R⊆(V-Σ)×[Σ(V-Σ)∪Σ]$.  ([[Concatenación de Cadenas]])
- $S$ es el símbolo inicial, un elemento de $V-Σ$
***
El [[Lenguajes Regulares|lenguaje]] generado por una gramática $G$, denotado $L(G)$, se define como$$L(G)=\{w∈Σ^*|S\dot⇒w\}\color{red}[1]$$
***
[[Derivación - Grámatica Regular]] 
[[Obtención de un AFD a partir de una Gramática Regular]] 
[1]. [[Clausura Reflexo Transitiva de la Derivación - Gramática Regular]] 