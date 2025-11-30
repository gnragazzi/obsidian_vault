#### Definición

> Una ***Máquina de Turing*** determinística, es una 6-upla $M=\langle Q,\Sigma,\Gamma,\delta,q_0,q_f\rangle$ donde:
> 	- $Q$: conjunto de estados
> 	- $\Sigma$: alfabeto de entrada
> 	- $\Gamma$: alfabeto de la cinta, con $\Sigma\subset\Gamma$
> 	- $\delta$: función de transición $$\delta:Q×\Gamma\to2^{Q×\Gamma×\{I,D,N\}}$$
> 	- $q_0$: estado inicial
> 	- $q_f$: estado final

#### Notas

- Existen varias especificaciones de la MT estándar.
	- Trabajamos con la MT que tiene un único estado final
- La cinta de la MT es infina a derecha.
- Inicialmente, una MT:
	- está en el estado $q_0$
	- La cabeza lecto/grabadora está apuntando al primer símbolo de $w$, la cadena de entrada
	- $w$ está ubicada en las primeras $|w|$ celdas de la izquierda.
	- El resto de las celdas (infinitas) contiene un símbolo especial *blanco*, denotado $B$, con $B\in\Gamma$

****
#### Etiquetas

#Anki 