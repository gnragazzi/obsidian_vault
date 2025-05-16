Si se trabaja con lenguajes con igualdad deben adicionarse dos reglas más:
$$R_{t_1 = t_2} \quad \frac{t_1 = t_2}{\varphi(x/t_1) \rightarrow \varphi(x/t_2)}$$
donde $\varphi$ es una [[Fórmulas Atómicas - LPO|fórmula atómica]] cualquiera,  
y $t_1$ y $t_2$ son [[Término - Lógica Primer Orden|términos]] sin variables.
$$R_{t = t} \quad t = t$$
donde $t$ es un término sin variables.
***
Estas reglas ponen cosas verdaderas en el árbol si la premisa era verdadera en $R_{t_1 = t_2}$, y en $R_{t = t}$ solo se agrega la conclusión.
Observar que la regla $R_{t = t}$ no necesita premisas para aplicarse, por lo tanto siempre se puede agregar, como único sucesor del nodo terminal de una rama de $\mathcal{A}$, un nuevo nodo al árbol conteniendo las conclusiones de la regla (o sea, $t = t$) para cualquier término de $L_\sigma^{Par}$ en el que no figuran variables.
***
Ejemplo 
![[Pasted image 20250513084150.png]]