### Definición Recursiva
$\hatδ:Q×Σ^*→2^Q$
Definición Recursiva de $\hatδ$
1. $\hatδ+(q,λ)=\{q\}$
2. $\hatδ(q,w)=\{r_1,r_2,...,r_m\}$
	1. $w=xσ$,
	2. $\hatδ(q,x)=\{p_1,p_2,...,p_k\}$ 
	3. $\bigcup\limits_{i=1}^{k} δ(p_i,σ)=\{r_1,r_2,...,r_m\}$
***
### Lenguaje que acepta
> Si $M$ es un [[Autómata Finito No Determinístico|AFND]], luego $$L(M)=\{w∈Σ^*|\hatδ(q_0,w)∩F≠∅\}$$
### Etiquetas
- #v2 