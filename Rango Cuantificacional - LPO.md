Llamaremos _rango cuantificacional_ de una [[Fórmula - LPO|fórmula]] $\varphi$ de $L_{\sigma}$, y lo denotaremos como $Rq(\varphi)$, al máximo número de [[Alfabeto - LPO#^638c55|cuantificadores]] anidados que figuran en $\varphi$.
Observemos que:
- Si $\varphi$ es una [[Fórmulas Atómicas - LPO|fórmula atómica]]        $$Rq(\varphi) \overset{\text{def}}{=} 0.$$
- En cualquier otro caso, si $\varphi$ y $\psi$ son fórmulas:
    $$Rq(\neg \varphi) \overset{\text{def}}{=} Rq(\varphi).$$ $$Rq((\varphi \lor \psi)) = Rq((\varphi \land \psi)) = Rq((\varphi \rightarrow \psi)) \overset{\text{def}}{=} \max\{Rq(\varphi), Rq(\psi)\}. $$
    $$Rq((\forall x\ \varphi)) = Rq((\exists x\ \varphi)) \overset{\text{def}}{=} Rq(\varphi) + 1.$$
***
![[Pasted image 20250507071706.png]]