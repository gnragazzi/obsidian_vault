#### Definición
- Si $G_{AB}$ es ambigua, entonces existen varias secuencias de derivaciones que, partiendo de $S$, producen una cadena $w$.
	- Como ya se ha visto, una misma cadena de símbolos terminales no puede tener más de una derivación en $G_A$ ni más de una derivación en $G_B$ (no son ambigüas).
- Luego, la única forma en que una cadena tenga dos derivaciones que concluyan en la misma cadena es que una comience con $S\Rightarrow A$ y continue con una secuencia de derivaciones en $G_A$; mientras que la otra debería comenzar con $S\Rightarrow B$ y continuar con una secuencia de derivaciones en $G_B$.
- La cadena con 2 derivaciones tienen una secuencia de índices $a_{i_m}...a_{i_2}a_{i_1}$ para algún $m\ge1$. Esta "cola" es una [[Solución PCP|solución]] a la [[Instancia PCP]], puesto que lo que precede la cola en la cadena con dos derivaciones es, al mismo tiempo, $w_{i_1}w_{i_2}...w_{i_m}$ y $x_{i_1}x_{i_2}...x_{i_m}$.

![[Pasted image 20251205224529.png]]
***
#### Etiquetas
- #falta 
