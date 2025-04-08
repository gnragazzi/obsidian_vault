Da un procedimiento recursivo para descubrir estados distiguibles en un [[Autómata Finito Determinístico|AFD]] $M=(...)$
- Base
	- Si $p$ es un estado final y $q$ es un estado no final, entonces el par $\{p,q\}$ es distinguible.
- Inducción:
	- Sean $p$ y $q$ estados tales que para algún símbolo de entrada $a$, $\delta(p,a)=r$ y $\delta(q,a)=s$, si $r$ y $s$ son un par de estados distinguibles, entonces el par $\{p,q\}$ es un par de estados distinguibles, también.
***
Ejecución![[Pasted image 20250407202442.png]]
![[Pasted image 20250407202456.png]]

***
[[Testeo de Estados Equivalentes]] 