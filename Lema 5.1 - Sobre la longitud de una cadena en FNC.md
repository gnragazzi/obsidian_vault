### Lema

Sea $G$ una gramática en $FNC$ y $A\Rightarrow^*w$ una derivación para $w\in\Sigma^*$, con un árbol de derivación $T$. Si la profundidad de $T$ es igual a $n$, entonces $|w|≤2^{n-1}$.

### Demostración por inducción en la profundidad de T
- Caso base $n=1$
	- ![[Pasted image 20250720110137.png]]
- Caso inductivo
	- Hipótesis inductiva: se cumple que para todo árbol de derivación de una profundidad $k$, la longitud de dicha cadena es mayor o igual a $2^{k-1}$.
	- Sea  $A\Rightarrow^*w$ una derivación para $w\in\Sigma^*$, con árbol de derivación T de profundidad k+1
	- Como G está en FNC, 
		- existe una producción de la forma $A\Rightarrow BC$. 
		- existen derivaciones $B\Rightarrow^*u$ y $C\Rightarrow^*v$, con $u,v\in \Sigma^*$, con $w=uv$
		- $T$ tiene como subárbol izquierdo al árbol $T_B$ y $T$ tiene como subárbol derecho al árbol $T_C$, ambos de profundidad k.
			- ![[Pasted image 20250720110243.png]]
		- Luego, por hipótesis inductiva $|u|≤2^{k-1}$ y $|v|≤2^{k-1}$ 
			- $|u|+|v| ≤ 2^{k-1} + 2^{k-1}$
			- $|uv| ≤ 2*2^{k-1}$
			- $|w| ≤ 2^{k}$
				- que era lo que quería probar

***
#v2 