#### Definición

> Un autómata linealmente acotado es una 6-upla $M=\langle Q,\Sigma,\Gamma,\delta,q_0,F\rangle$ donde:
> 	- $Q$: conjunto de estados
> 	- $\Sigma$: alfabeto de entrada
> 	- $\Gamma$: alfabeto de la cinta, con $\Sigma\subseteq\Gamma$
> 	- $\delta$: función de transición $$\delta:Q×\Gamma\to2^{Q×\Gamma×\{I,D\}}$$
> 	- $q_0$: estado inicial
> 	- $F\subseteq Q$: conjunto de estados finales

***
#### Notas

- El autómata tiene una cabeza lecto/grabadora que permite movimientos a izquierda y a derecha en la cinta
	- $I$ representa un movimiento a izquierda en la cinta
	- $D$ representa un movimiento a derecha en la cinta
- $\Sigma$ contiene los símbolos $\#$ y $\$$ que representan, respectivamente, los límites izquierdo y derecho de la cinta.
	- ![[Pasted image 20250723085823.png]]
	- ![[Pasted image 20250723085837.png]]

***
#### Etiquetas

#v2 