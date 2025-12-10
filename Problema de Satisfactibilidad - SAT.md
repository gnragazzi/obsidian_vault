#### Definición
Sea $\mathcal{F}=C_1\land C_2\land ...\land C_m$ donde 
- $C_i=(y_{i1}\lor...\lor y_{ik})$
- $y_{ij}\in(X\cup\overline{X})$ 
El problema consiste en determinar si existe al menos una asignaciones de valores de verdad a las variables en $X=\{x_1,...,x_n\}$ que [[Satisfacible|satisfagan]] a las proposiciones en $\mathcal{F}$.

#### Lenguaje Asociado
$$L_{SAT}=\{\langle\mathcal{F}\rangle/\mathcal{F}\text{ es satisfecha por alguna asignación de valores de verdad a las variables de }\mathcal{F}\}$$
***
#### Posible Algoritmo para una MTND que decida SAT

![[Pasted image 20251209170925.png]]
****
#### Posible Algoritmo para una MTD que decida SAT

![[Pasted image 20251209171053.png]]
***
#### SAT es NP-Completo

El [[Teorema de Cook]] demuestra que
- $L_{SAT}\in\mathcal{NP}$
- $L_{SAT}\in\mathcal{NP}-hard$
	- $\Rightarrow$ $L_{SAT}\in\mathcal{NP}-completo$
***
#### Etiquetas
- #falta 