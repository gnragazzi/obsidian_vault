#### Demostración
- Construimos una [[Máquina de Turing no Determinística - MTND|MTND]] que
	- Tome como entrada la representación binaria de una [[Máquina de Turing Determinista - MT (MTD)|MT]], $M_i$.
	- "Adivine" mediante el no-determinismo una cadena $w$ que $M_i$ podría aceptar (todas las cadenas que podría aceptar al mismo tiempo)
	- $M$ prueba, mediante la [[Máquina de Turing Universal (MT U)]], el par $\langle M_i,w\rangle$ 
		- Si $w\in M_i$, la MTU acepta la cadena y $M$ acepta a $M_i$ ($M_i\in$ [[Lne]])

![[Pasted image 20251205233606.png]]

De esta manera, observamos que si $M_i$ acepta aunque sea una entrada, $M$ adivinará dicha entrada y aceptará $M_i$. Caso contrario, si $M_i$ no acepta ninguna entrada, no habrá cadena "adivinada" por $M$ que conlleve la aceptación de $M_i$. Luego $L(M)=L_{ne}$.

***
#### Etiquetas
- #Anki 