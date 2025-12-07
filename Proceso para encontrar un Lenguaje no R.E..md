#### Procedimiento
Queremos encontrar un lenguaje no [[Lenguajes Recursivamente Enumerables|R.E.]]. Para ello, partimos del conocimiento de que [[MT como forma de demostrar que un lenguaje es o no R.E.|un lenguaje L es R.E. si existe una MT M tal que L=L(M)]].
1. Utilizando el [[Orden Canónico|orden canónico]], listamos todas las cadenas de $\{0,1\}^*$.
	1. De esta manera, cada cadena listada es asociada a un entero (enumeración). Luego $x_1=\lambda, x_2=0, x_3=1, x_4=00, x_5=01,$ etc...
2. Cada una de estas cadenas $x_i$, con $i=1,2,...$, [[Codificación de una MT usando {0,1}*|representa una MT]]. De esta manera, podemos hablar de la *i-ésima* MT, $M_i$, que es la representada por la cadena $x_i$.
	1. Recordamos que, cuando la cadena en cuestión no es una representación bien formada, la MT correspondiente describe un lenguaje vacío.
3. Construimos una matriz A con infinitas filas e infinitas columnas tal que:
	1. cada fila i representa al vector característico del lenguaje $L_i=L(M_i)$. 
	2. Cada entrada de la matriz $a_{i,j}$ es definida como $$a_{i,j}=\begin{cases}0&\text{si }x_j\notin L(M_i)\\1&\text{si }x_j\in L(M_i)\end{cases}$$
	3. Podemos ver un **ejemplo simplificado**:
		1. ![[Pasted image 20251130112638.png|400]]
4. Definimos un nuevo lenguaje $L_d$, ([[Lenguaje de la Diagonal]]), como $$L_d=\{x_i\in\{0,1\}^* / x_i\notin L(M_i)\}$$
5. Como $L_d$ se obtiene complementando la diagonal de la matriz definida anteriormente, observamos que $L_d\ne L(M_i)$ para todo $i=1,2,...$
	1. Esto se observa claramente en el vector característico (construido de manera similar que antes) de $L_d$: este se diferenciará (al menos) en el i-ésimo elemento del vector característico de cualquier otro lenguaje $L_i$.
	2. ![[Pasted image 20251130114959.png|500]]
6. Esto nos da un lenguaje $L_d$ que no es R.E. 
***
#### Etiquetas
- #falta 