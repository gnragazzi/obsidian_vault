#### Definición
- Construimos una [[Máquina de Turing no Determinística - MTND|MTND]] que
	- Tome como entrada la representación binaria de una [[Máquina de Turing Determinista - MT (MTD)|MT]], $M_i$.
	- "Adivine" mediante el no-determinismo una cadena $w$ que $M_i$ podría aceptar (todas las cadenas que podría aceptar al mismo tiempo)
	- $M$ prueba, mediante la [[Máquina de Turing Universal (MT U)]], el par $\langle M_i,w\rangle$ 
		- Si $w\in M_i$, la MTU acepta la cadena y $M$ acepta a $M_i$ ($M_i\in$ [[Lne]])

![[Pasted image 20251205233606.png]]
***
#### Etiquetas
- #falta 