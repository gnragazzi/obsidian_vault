#### Definición

> Una ***Máquina de Turing*** determinística, es una 6-upla $M=\langle Q,\Sigma,\Gamma,\delta,q_0,q_f\rangle$ donde:
> 	- $Q$: conjunto de estados
> 	- $\Sigma$: alfabeto de entrada
> 	- $\Gamma$: alfabeto de la cinta, con $\Sigma\cup\{\mathbb{B}\}\subseteq\Gamma$
> 	- $\delta$: función de transición $$\delta:Q×\Gamma\to{Q×\Gamma×\{I,D,N\}}$$
> 	- $q_0$: estado inicial
> 	- $q_f$: estado final

***
#### Notas
- Existen varias especificaciones de una MT-Estandar, pero todas ellas son equivalentes:
	- Pueden tener más de un estado final o incluso no tener estado final
	- Pueden no tener $N$, es decir `NO-OP`
***
#### Etiquetas
#Anki 