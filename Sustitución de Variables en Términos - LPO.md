Sean $s$ y $y$ [[Término - Lógica Primer Orden|términos]] de un [[Alfabeto de la Lógica de Primer Orden|lenguaje]] $L_\sigma$, y sea $x$ una variable. Con $t(x/s)$ designamos al término que se obtiene sustituyendo en $t$ todas las apariciones de la variable $x$ por el término $s$. Más precisamente, $t(x/s)$ se define por inducción en la complejidad de $t$ del modo siguiente:
1. Sea $comp(t)=0$, entonces t es una constante o una variable. Si $t$ es una constante, no hay nada que sustituir; en otro caso, si $t$ es distinto que $x$, entonces el término no cambia, es decir que $t(x/s)$ es $t$. Si $t$ es la variable $x$, entonces t(x/s) cambia a $s$.
2. Sea $comp(t)=n>0$ y supongamos que hemos definido $u(x/s)$ para todo término $u$ tal que $comp(u)<n$. Entonces, hay un único $k≥1$ un único $f\in\mathcal{F}$ de aridad $k$ y una única k-upla de términos $t_1,...,t_k$ tales que $t=f(t_1,...,t_k)$. Como $comp(t_i)<comp(t)=n$, por la hipótesis inductiva está definida $t_i(x/s)$ para $i=1,2,...,k$, luego $$t(x/s) \text{ es }f(t_1(x/s),...,t_k(x/s))$$
***
La sustitución de variables no se puede realizar sobre  cualquier variable. Se restringe la sustitucion únicamente a variables que [[Apariciones Libres y Ligadas de Variables|figuren libres]] en una [[Fórmulas de la Lógica de Primer Orden|fórmula]]. 
Asimismo, esa variable solo puede ser sustituida por otra variable libre.
os restringiremos a sustituir sólo variables libres por términos sin variables
***
- [[Grado de Complejidad de una fórmula - LPO]]
- 