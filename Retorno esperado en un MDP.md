El retorno, que denotaremos $R_t$ se define en función de la secuencia de recompensas $r_{t+1},r_{t+2},...$ acumulándolas en base a algún criterio particular.
Uno de los enfoques más utilizados es sumar cada recompensa, pero decrementarla geométricamente de acuerdo a un *factor de descuento* $\gamma$ (donde $0≤\gamma≤1$) y el número de pasos transcurridos hasta que se recibió la recompensa.
En este caso diremos que $R_t$ es el ***retorno decrementado*** y que el agente ***maximiza*** el ***retorno decrementado esperado***:
$$E\{R_t\}=E\{r_{t+1}+\gamma r_{t+2}+\gamma² r_{t+2}+...\}=E\{\sum_{k=0}^\infty\gamma^kr_{t+k+1}\}$$
- 