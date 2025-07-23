#### Definición

Una gramática Dependiente del contexto es aquella 4-upla $G=\langle N,\Sigma,P,S\rangle$, cuyo conjunto P consiste en producciones que respetan la [Propiedad no-decreciente], y son de la forma:$$\alpha A\beta\to\alpha\gamma\beta\text{ donde }\alpha,\beta\in(N\cup\Sigma)^*,A\in N, \gamma\in(N\cup\Sigma)⁺$$
(La única producción que permite $\lambda$ es $S\to\lambda$, siempre que $S$ no aparezca del lado derecho de ninguna producción).

***
#### Propiedad no-decreciente

Una producción es ***no decreciente*** si la longitud de cualquier cadena que se obtiene de ella es no-decreciente, es decir que si $\alpha\to\beta$, entonces $|\alpha|\le|\beta|$. 

***

- [[Recursividad de las GDC]] 

***
#### Interpretación

- Es decir, el lado izquierdo de una producción debe tener al menos un no terminal, pero puede ser una palabra entera (a diferencia de las [[Gramáticas Libres del Contexto - GLC|GLC]]) y el resultado puede ser cualquier cadena a excepción de $\lambda$, SIEMPRE QUE ESTA CADENA RESPETE EL CONTEXTO.
	- Por ejemplo:
		- ![[Pasted image 20250722083256.png]]

***
#### Etiquetas
#v2 