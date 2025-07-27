#### Teorema: 

> Si una Gramática es dependiente/sensitiva del contexto, entonces es [[Gramática Recursiva|recursiva]]

***

#### Demostración

1. Sea $G=\langle N,\Sigma,P,S\rangle$ una GDC
2. Determinar por inspección si $\lambda\in L(G)$ y remover $S\to\lambda$ del conjunto de producciones y asumir que P no contiene la producción $S\to\lambda$.
3. Sea 
	1. $w\in\Sigma^+$, con $|w|=n$.
	2. $V=N\cup\Sigma$ 
	3. $T_m=\{\alpha\in V⁺ : |\alpha|\le n \land S\Rightarrow^k\alpha, k\le m\}$, con 
4. Luego, 
	1. $T_0=\{S\}$ y
	2. $T_m$ se puede calcular a partir de $T_{m-1}$, viendo que cadenas de longitud menor o igual a n pueden ser derivadas desde cadenas en $T_{m-1}$ por la aplicación de una producción. Es decir $$T_m=T_{m-1}\cup\{\alpha : \beta\in T_{m-1},\beta\Rightarrow\alpha,|\alpha|\le n\}$$
5. Es evidente que $T_{m-1}\subseteq T_m$ para $m\ge1$.
	1. Dado que $T_m$ depende solo de $T_{m-1}$, si $T_{m-1}=T_{m}$, entonces $T_{m}=T_{m+1}=T_{m+2}=...$
	2. Nuestro algoritmo será calcular $T_1,T_2,...$ hasta que, para algún $m$, $T_{m}=T_{m-1}$
	3. Si 
		1. $w\in T_m \rightarrow w\in L(G)$ y $S\Rightarrow^* w$ 
		2. $w\notin T_m \rightarrow w\notin L(G)$   
 