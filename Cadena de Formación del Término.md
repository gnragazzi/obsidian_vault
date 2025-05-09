Una _cadena de formación del [[Término - Lógica Primer Orden|término]]_ $t_n$ es una [[Sucesión|sucesión]] finita $t_1, \ldots, t_n$ de elementos de $A^*$ que satisface las siguientes condiciones:
- **(CFT)** Para cada $i$ tal que $1 \leq i \leq n$, se tiene que:
	- o bien $t_i$ es un símbolo de [[Alfabeto - LPO#^638c55|variable]].
    - o bien $t_i$ es un símbolo de [[Alfabeto - LPO#^638c55|constante]].
    - o bien existen un símbolo de función $k$-aria $f$ y $k$ índices $i_1, \ldots, i_k$, todos estrictamente menores que $i$, tales que $t_i$ es $f(t_{i_1}, \ldots, t_{i_k})$.
El subíndice $n \geq 1$ del último término será llamado _longitud_ de la cadena de formación.