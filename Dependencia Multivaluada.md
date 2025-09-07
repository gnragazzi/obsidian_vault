#### Definición
- Sean:
	- $R=\{A_1,A_2,...,A_2\}$ donde 
		- $R$ es una relación (tabla)
		- $A_i$ es un atributo de la relación.
	- $X,Y\subseteq R$
		- Es decir, $X,Y$ son conjuntos de atributos de $R$
- Una dependencia multivaluada (o dmv) $X\rightarrow\rightarrow Y$ especifica la siguiente restricción para cualquier instancia $r$ de $R$
	- Si existen dos tuplas $t_i,t_j\in r$ tales que $t_i(X)=t_j(X)$, entonces existen dos tuplas $t_k,t_p$ tales que:
		- $t_i​(X)=t_j​(X)=t_k​(X)=t_p​(X)$    
		- $t_i​(Y)=t_k​(Y)\text{ y }t_j​(Y)=t_p​(Y)$    
		- $t_j​(R−XY)=t_k​(R−XY)\text{ y }t_i​(R−XY)=t_p​(R−XY)$
- En tal caso, decimos que $X$ multidetermina a $Y$ (o que $Y$ multidepende de $X$) y, dado que $Y$ y $R-XY$ son independientes entre si, lo denotamos como$$X\rightarrow\rightarrow Y/R-(XY)$$
***
- [[Descomposición sin Pérdida de Información para 4FN]]	
- [[Reglas de Inferencia para las DMV]] 
***
#### Etiquetas
- #falta 