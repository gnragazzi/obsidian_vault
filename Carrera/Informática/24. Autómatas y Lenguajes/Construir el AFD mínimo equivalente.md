A partir de M, construimos un [[Autómata Finito Determinístico|AFD]] N usando los bloques como sus estados.
1. El estado inicial de N es el bloque que contiene el estado inicial de M.
2. El conjunto de estados finales de N es el conjunto de bloques que contienen estados finales de M
3. La función de transición de N, a la cual llamaremos $\gamma$, se define de la siguiente manera:
	1. Supongamos $S$ un conjunto de estados equivalentes de $M$, sea $a∈\Sigma$, entonces debe existir un bloque $T$ de estados tal que $$∀q∈S:\delta(q,a)∈T$$Como consecuencia, podemos escribir $\gamma(S,a)=T$ 
