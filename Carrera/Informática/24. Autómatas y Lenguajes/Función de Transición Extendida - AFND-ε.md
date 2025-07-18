### Definición Formal

1. $\hat\delta(q,ε)=\text{clausura-}ε(q)$
2. Suponemos que w es de la forma $xa$, donde $a$ es el último símbolo de $w$, con $a∈Σ$, (por lo tanto, $a≠ε$). Entonces computamos $\hat\delta(q,w)$ según los siguientes 3 pasos:
	1. Sea $\hat\delta(q,x)=\{p_1,p_2,...,p_k\}$
	2. Sea $\bigcup\limits_{i=1}^{k} δ(p_i,a)=\{r_1,r_2,...,r_m\}$ 
	3. Entonces $\hat\delta(q,w)=\bigcup\limits_{j=1}^{m}\text{clausura-}e(r_j)\color{violet}^{[1]}$ 
***
### Lenguaje definido por un AFND-ε

> Sea $E=(Q,Σ,δ,q_0,F)$ un [[AFND-ε]], se define el lenguaje aceptado por $E$ como$$L(E)=\{w∈Σ^*
|\hat\delta(q_0,w)∩F≠∅\}$$
***
### Pasos para resolver la función de transición extendida


> Aunque se llega siempre a la respuesta correcta usando el camino recursivo desde el inicio, en el libro resume todos los pasos partiendo directamente desde el cálculo de la clausura-ε con el estado inicial y recorriendo el camino desde el primer símbolo hasta el final de la cadena.
![[Pasted image 20250329151430.png]]
***
[1]. [[Clausura ε]] 

### Etiquetas

#v2 