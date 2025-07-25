- ## Definición
	 - Sea $L_{ER}$ es el conjunto de todas las posibles [[Expresiones Regulares - Lenguajes|expresiones regulares]]. Entonces definimos la ***función de valuación*** $$ϕ:L_{ER}→2^{Σ^*}\color{red}[1]$$como aquella que toma como argumento una [[Definición Recursiva de E.R.|expresión regular bien formada]] y da como resultado el conjunto de cadenas denotado por dicha expresión regular. 
- ## Definición Recursiva
	- Sean $E,F\in L_{ER}$. Entonces:
		- $ϕ(∅) = \{\}$ el conjunto vacío
		- $ϕ(λ) = \{λ\}$ el conjunto formado por la [[Cadena - Lenguajes#^41d68b|cadena de longitud nula]].
		- $ϕ(a) = \{a\}$ el conjunto formado por la cadena $a$.
		- $ϕ(E.F) = ϕ(E).ϕ(F)$ el conjunto formado por la concatenación de conjuntos.
		- $ϕ(E+F) = ϕ(E)∪ϕ(F)$ el conjunto formado por la concatenación de conjuntos.
		- $ϕ(E*) = ϕ*(E)$ clausura de un conjunto
		- $ϕ((E)) = ϕ(E)$ 
- ## Etiquetas
	- #v2 
- ## Notas
	- [1]. [[Conjunto de Partes#^d7cf39|Notación Alternativa para el conjunto de partes]]