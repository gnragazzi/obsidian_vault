Da un procedimiento recursivo para descubrir [[Testeo de Estados Equivalentes#^f07b74|estados distiguibles]] en un [[Autómata Finito Determinístico|AFD]] $M=(...)$
- Base
	- Si $p$ es un estado final y $q$ es un estado no final, entonces el par $\{p,q\}$ es distinguible.
- Inducción:
	- Sean $p$ y $q$ estados tales que para algún símbolo de entrada $a$, $\delta(p,a)=r$ y $\delta(q,a)=s$, si $r$ y $s$ son un par de estados distinguibles, entonces el par $\{p,q\}$ es un par de estados distinguibles, también.
		- Lo que nos quiere decir es que, siendo $w\in \Sigma^*$ si solamente uno de $\hat\delta(r,w)$ y $\hat\delta(s,w)$ es un estado final, entonces es claro que solamente uno entre $\hat\delta(p,aw)$ y $\hat\delta(q,aw)$ lo será.
***
Ejecución![[Pasted image 20250407202442.png]]
![[Pasted image 20250407202456.png]]

***
[[Testeo de Estados Equivalentes]] 