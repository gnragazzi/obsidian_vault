#### Definición
> Una configuración correspondiente a una [[Máquina de Turing - Determinista|MT]] $M=\langle Q,\Sigma,\Gamma,\delta,q_0,q_f\rangle$ es una cadena $$z=\alpha p\beta$$
> donde $\alpha,\beta\in\Gamma^*$ y $p\in Q$.

#### Cómo interpretar una Configuración

Sea $\alpha p\beta$ una configuración, entonces $M$ procede de alguna de las siguientes maneras:
1. Si $p=q_f$, $M$ se detiene y [[Criterios de Aceptación-Rechazo de una MT Estándar|acepta]] 
2. Si $\beta=\lambda$, la cabeza lecto/grabadora de $M$ está sobre una celda con símbolo $\mathbb{B}$ y si $$\delta(p,\mathbb{B})=\{q,X,T\} \text{ (con }p,q\in Q, X\in\Gamma, T\in \{I,D,N\})$$se tiene que:
	1. en la cinta se reemplaza $\mathbb{B}$ con $X$, 
	2. La cabeza se mueve según la dirección $T$,
	3. M entra en el estado $q$
3. Si $\beta=a\beta'$, con $a\in\Gamma,\beta'\in\Gamma^*$ y $$\delta(p,a)=\{q,X,T\} \text{ (con }p,q\in Q, X\in\Gamma, T\in \{I,D,N\})$$se tiene que:
	1. en la cinta se reemplaza $a$ con $X$, 
	2. La cabeza se mueve según la dirección $T$,
	3. M entra en el estado $q$
4. Si para alguno de los casos anteriores, $\delta$ no está definida, la máquina se detiene sin aceptar.

#### Etiquetas
#Anki 
