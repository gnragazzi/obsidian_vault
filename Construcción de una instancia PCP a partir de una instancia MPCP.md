#### Definición
- Dada la [[Instancia MPCP|Instancia de MPCP]]
	- $A=w_1,w_2,...,w_k$ 
	- $B=x_1,x_2,...,x_k$
- Asumiendo que los símbolos $*, \$\notin\Sigma$ , construimos la [[Instancia PCP]] de la siguiente manera:
	- $C=y_0,y_1,y_2,...,y_k,y_{k+1}$ donde 
		- para $i=1,2,...,k$ si $w_i=\sigma_1\sigma_2...\sigma_n$, entonces $y_i$ se define como $y_i=\sigma_1*\sigma_2*...\sigma_n*$, es decir que $y_i$ se construye a partir de $w_i$, agregándole un símbolo $*$ después de cada símbolo $\sigma\in\Sigma$ de $w_i$.
		- $y_0=*y_1$
		- $y_{k+1}=\$$ 
	- $D=z_0,z_1,z_2,...,z_k,z_{k+1}$ donde
		- para $i=1,2,...,k$ si $x_i=\sigma_1\sigma_2...\sigma_n$, entonces $z_i$ se define como $z_i=*\sigma_1*\sigma_2...*\sigma_n$, es decir que $z_i$ se construye a partir de $x_i$, agregándole un símbolo $*$ antes de cada símbolo $\sigma\in\Sigma$ de $x_i$.
		- $z_0=z_1$
		- $z_{k+1}=*\$$ 
		
***
#### PCP se [[Reducción (de un problema A a un problema B)|reduce]] a MPCP (Demostración)

1. Supongamos que $i_1,i_2,...,i_m$ es una [[Solución MPCP|solución]] a la instancia dada de MPCP. Sabemos entonces que $$w_{i_1}w{i_2}...w_{i_m}=x_{i_1}x_{i_2}...x_{i_m}$$
2. Si reemplazamos las $w$'s y $x$'s por $y$'s y $z$'s, entonces tendriamos dos cadenas casi iguales, a excepción del símbolo $*$ al comienzo de $z$ y al final de $y$. Por ello, podemos afirmar que $$*y_{i_1}y{i_2}...y_{i_m}=z_{i_1}z_{i_2}...z_{i_m}*$$
3. Como $y_0=*y_1$ y $z_0=z_1$, podemos afirmar que$$y_0y_{i_1}y{i_2}...y_{i_m}=z_0z_{i_1}z_{i_2}...z_{i_m}*$$
4. Sabiendo que $y_{k+1}=\$$ y $z_{k+1}=*\$$$$y_0y_{i_1}y{i_2}...y_{i_m}y_{k+1}=z_0z_{i_1}z_{i_2}...z_{i_m}z_{k+1}$$ y ahora tenemos una solución al MPCP.
Ahora es necesario mostrar que si la instancia construida del PCP tiene una [[Solución PCP|solución]], entonces el MPCP que se utilizó para la reducción, también la tiene.
- Observemos que, por cómo está construido, una solución al PCP comenzará con $i_0$ y terminará con $i_{k+1}$, así que la solución será de la forma $$0,i_1,i_2,...,i_m,i_{k+1}$$
- Afirmamos que $i_1,i_2,...,i_m$ es una solución para la instancia del MPCP. La razón es que si removemos los símbolos $*,\$$ de la cadena $y_{i_1}y{i_2}...y_{i_m}$, obtenemos la cadena $w_{i_1}w{i_2}...w_{i_m}$. De igual manera, si removemos $*,\$$ de $z_{i_1}z{i_2}...z_{i_m}$, obtenemos $x_{i_1}x{i_2}...x_{i_m}$.
- Sabemos que $$y_0y_{i_1}y{i_2}...y_{i_m}y_{k+1}=z_0z_{i_1}z_{i_2}...z_{i_m}z_{k+1}$$así que se $$w_{i_1}w_{i_2}...w_{i_m}=x_{i_1}x_{i_2}...x_{i_m}$$
***
#### Etiquetas
- #Anki  