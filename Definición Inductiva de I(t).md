Dada una [[Interpretación - Definición LPO|interpretación]] $\mathcal{I}$ del [[Alfabeto de la Lógica de Primer Orden|vocabulario]] $\sigma$ para el lenguaje $L_\sigma$, vamos a definir, por [[Principio de Inducción Matemática|inducción]] en el [[Grado de Complejidad de un Término|grado de complejidad]] de los [[Término - Lógica Primer Orden|términos]], una interpretación $\mathcal{I}(t) \in U$ para los términos $t$ de $L_\sigma$ del modo siguiente:
1. Sea $comp(t) = 0$, luego $t$ puede ser una variable o una constante. 
	1. Sea $t$ una constante igual a $c \in \mathcal{C}$. Definimos:  
    $$\mathcal{I}(t) \text{ como }c^{\mathcal{I}} \in U \text{ (o equivalentemente }\mathcal{I}(t)\text{ como }\alpha(c) \in U).$$
2. Sea $comp(t) = n > 0$ y supongamos que hemos definido $\mathcal{I}(s)$ para todo término $s$ de complejidad menor que $n$. Si $t$ es un término de complejidad $n$, entonces hay un único $k \geq 1$, un único símbolo $f \in \mathcal{F}$ de aridad $k$ y una única $k$-upla de términos $(t_1, \ldots, t_k)$ tales que $t = f(t_1, \ldots, t_k)$. Como $comp(t_i) < comp(t) = n$, por la hipótesis inductiva están definidas las interpretaciones $\mathcal{I}(t_i) \in U$ para $i = 1, 2, \ldots, k$. 
	1. Entonces definimos $\mathcal{I}(t)$ del modo siguiente:
    $$\mathcal{I}(t) = f^{\mathcal{I}}(\mathcal{I}(t_1), \mathcal{I}(t_2), \ldots, \mathcal{I}(t_k)) \in U$$
***
[[Proposición 1 - Equivalencia de interpretaciones]] 
***
Diremos que el término $t$ designa o nombra al elemento $I(t)$ del universo $U$. El superíndice $\mathcal{I}$  que acompaña a las constantes y a las funciones, nos dicen que ese es el elemento del universo o la  función total respectivamente, que la interpretación $\mathcal{I}$ asigna a los símbolos de constantes y de función que aparecen en el vocabulario. 
***
La definición anterior nos da un procedimiento para calcular $\mathcal{I}(t)$:
- reemplazar cada uno de los símbolos de constante que figuran en $t$ por los elementos del universo $U$ que les asigna la interpretación $\mathcal{I}$,
- ir aplicando sucesivamente a los elementos de $U$ así obtenidos las funciones que $I$ le asigna a los símbolos de función que figuran en $t$, en el orden en que aparecen.
***
![[Pasted image 20250507075456.png]]
![[Pasted image 20250507075518.png]]