#### Definición
- Supongamos que $g,h\in FRP$ donde
	- el dominio de $g$ es $\mathbb{N}^n$
	- el dominio de $h$ es $\mathbb{N}^{n+2}$
- Entonces el par de funciones 
	- $(1)$           $f(x,0)=g(x)$   (caso base)
	- (2)           $f(x,y+1)=h(x,y,f(x,y))$    (caso recursivo)
	define una FRP total con dominio en $\mathbb{N}^{n+1}$
- Para el caso especial donde $n=0$ se define
	- (1)           $f(0) = k$, con $k\ge0$ 
	- (2)           $f(y+1)=h(y,f(y))$    (caso recursivo)
***
#### Etiquetas
- #Anki 