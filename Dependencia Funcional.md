#### Definición
- Sean:
	- $R=\{A_1,A_2,...,A_2\}$ donde 
		- $R$ es una relación (tabla)
		- $A_i$ es un atributo de la relación.
	- $X,Y\subseteq R$
		- Es decir, $X,Y$ son conjuntos de atributos de $R$
- Entonces diremos que X ***determina funcionalmente*** a $Y$, y lo denotamos $X\rightarrow Y$, si y solo si para cualquier instancia $r$ de $R$, no existen dos tuplas en r que coinciden en $X$ y no coinciden en $Y$. Formalmente $$X\rightarrow Y ≝ \forall\;tiempo\;T,\forall\;instancia\;r_T,\forall\;u,v\in r_t$$$$\Pi_X(u)=\Pi_X(v)\Rightarrow\Pi_Y(u)=\Pi_Y(v)$$
#### Clave
- Si $X$ determina funcionalmente a $R$, entonces $X$ es clave de la relación.
***
#### Etiquetas
- #falta 