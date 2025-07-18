### Definición

Una gramática $G = (N, \Sigma, P, S)$ es ***libre de contexto (GLC)***, si sus producciones en $P$ tienen la siguiente forma: $A \rightarrow \alpha$, con $A \in N$ y $\alpha \in (N \cup \Sigma)^*$.
	- En este  contexto, $N$ es el conjunto de no terminales y $\Sigma$ es el conjunto de los terminales.
	- La notación $\rightarrow$ se lee produce y se utiliza para describir las reglas/producciones de $P$.

***
### Lenguaje Generado

> El lenguaje generado por una gramática $G = (N, \Sigma, P, S)$ (denotado $L(G)$) es:  
$$L(G) = \{ w \in \Sigma^*  |  S \Rightarrow^* w \}$$
***
### Características

- El nombre _"libre de contexto"_ se debe a que cada una de las producciones pueden ser aplicadas independientemente del contexto en donde aparezca un no terminal en una _forma sentencial_.
	- A diferencia de las [[Gramática Regular|gramáticas regulares]] 
- Su importancia radica en que permiten describir los aspectos sintácticos de los lenguajes de programación. Por lo tanto tienen un rol central en el contexto de [[Compiladores]].
***
### Enlaces

[[Derivación - Gramáticas Libres de Contexto]] 
[[Forma Sentencial - GLC]] 
[[BNF]] 
[[BNFE]]
[[Ambigüedad en GLC]]

### Etiquetas

#v2 