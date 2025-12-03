#### Definición

> Sea $M=\langle Q,\Sigma,\Gamma,\delta,q_0,q_f\rangle$ una [[Máquina de Turing Determinista - MT (MTD)|MT determinística]]. 
> Luego, para un par de [[Configuración - MT|configuraciones]] $\alpha p\beta$ y $\alpha'p'\beta'$, es posible escribir $$(\alpha p\beta)\vdash(\alpha'p'\beta')$$si se cumple que:
> 	1. $\beta=A\gamma$ donde
> 		1. o bien $\beta=\lambda$ y, por convención $A=\mathbb{B},\gamma=\lambda$
> 		2. o bien $\beta\ne\lambda$ y $A\in\Gamma,\gamma\in\Gamma^*$ 
> 	2. $\delta(p,A)$ está definida y $p\ne q_f$ 
> 	3. $\delta(p,A)=(p',X,T)$ y uno se los siguientes puntos se cumplen:
> 		1. $T=I$, $\alpha=\alpha'C$, para algún $C\in\Gamma$ y $\beta'=CX\gamma$ 
> 		2. $T=N$, $\alpha=\alpha'$ y $\beta'=X\gamma$ 
> 		3. $T=D$, $\alpha'=\alpha X$ y $\beta'=\gamma$ 

***
#### Etiquetas
- #Anki 