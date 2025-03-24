Las ER utilizan las operaciones de unión (+), [[Concatenación de Cadenas|concatenación]] (.) y clausura de  Kleene $(^*)$.  Una ER sobre algún [[Alfabeto|alfabeto]] Σ se define recursivamente de la siguiente  manera:

- $∅$ es una [[Expresiones Regulares - Lenguajes|ER]] y denota el [[Conjuntos|conjunto]] vacío, $L(∅)=∅$
- $λ$ es una ER y denota el conjunto $\{λ\}$. $L(λ)=\{λ\}$
- $∀a∈Σ, a$ es una ER y denota el conjunto $\{a\}$. $L(a) = \{a\}$
- Si $ɑ$ y $β$ son ER, entonces:
	- $ɑ+β$ es una ER y denota el conjunto $L(ɑ+β)=L(ɑ) ∪ L(β)$.
	- $ɑβ$ es una ER y denota el conjunto $L(ɑβ)=L(ɑ)L(β)$.
	- $ɑ*$ es una ER y denota el conjunto $L(ɑ*)=(L(ɑ))*$.
	- $ɑ$ es una ER y denota el conjunto $L((ɑ))=L(ɑ)$.
***
[[Ejemplo de Expresiones Regulares]] 