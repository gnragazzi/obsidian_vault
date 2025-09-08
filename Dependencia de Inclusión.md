#### Definición
- Formaliza el concepto de ***Integridad Referencial***
- Dados dos esquemas de relación $R,S$ y dos conjuntos de atributos $X,Y$ donde $X\subseteq R,Y\subseteq S$ una ***dependencia de inclusión*** entre los dos conjuntos de atributos, denotada $R.X < S.Y$ especifica que para cualquier instancia válida $r$ para $R$ y cualquier instancia válida $s$ para S, se cumple que $$\Pi_X(r)\subseteq\Pi_Y(s)$$
***
#### Condiciones
- $X$ e $Y$ deben tener la misma cardinalidad
- Los dominios de los atributos de $X$ e $Y$ deben ser compatibles
	- Si $X=\{x_1,x_2,...,x_n\}$ y $Y=\{y_1,y_2,...,y_n\}$, entonces $dom(x_i)$ debe ser compatible con $dom(y_i)$ para $1\le i\le n$ 


***
#### Referencias
[[Proyección (álgebra relacional)]]
***
#### Etiquetas
- #Anki 