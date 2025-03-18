Una cadena de formación de longitud $n$ es una sucesión finita $X_1, X_2, . . . , X_n$ de elementos de $A^∗$ que satisface las condiciones siguientes:  
(CF) Para cada $i$, con $1 ≤ i ≤ n$, se tiene que:  
- o bien $X_i$ es una variable proposicional, 
- o bien existe un $j$ tal que 1 $≤ j ≤ i − 1$ y $X_i = ¬X_j$, 
- o bien existen $j$ y $k$, ambos entre $1 ≤ j$, $k ≤ i − 1$, tales que
	- $X_i = (X_j ∨ X_k)$  o
	- $X_i = (X_j ∧ X_k)$ o 
	- $X_i = (X_j → X_k)$
***
Cada uno de los $X_i$, con $1 ≤ i ≤ n$, es llamado ***eslabón*** de la cadena de formación.
***
Ejemplo:
$$P = (((p_0 ∨ p_1) → ¬p_3) ∧ p_0).$$
$$\matrix{
X_1 = p_0\\
X_2 = p_1\\  X_3 = p_3\\  X_4 = ¬X_3\\  X_5 = (X_1 ∨ X_2)\\  X_6 = (X_5 → X_4)\\  X_7 = (X_6 ∧ X_1)}$$
Notesé que **en este caso en particular**, la asignación de elementos a los eslabones (ya sean conectivos o [[Variables Proposicionales|variables]]) está dada por:
- Primero variables de izquierda a derecha
- Despues conectivos por orden de precedencia.
***
Propiedades:
- [[Irreducibilidad - Cadenas de Formación]] 
	- Haciendo un breve análisis pude observar que una cadena de formación es una colección de símbolos, pero únicamente es importante que el último eslabón sea igual a la [[Fórmula Lógica|fórmula]] para que cumpla con ser una. 
	- Es decir que en cualquiér eslabón anterior al último pueden haber eslabones que no estén presentes en la fórmula y seguir siendo una cadena de formación válida.
	- 