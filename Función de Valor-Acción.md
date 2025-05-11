El valor de la acción $a$ en el estado $s$, que denotaremos $Q^π(s, a)$, es el retorno esperado cuando se comienza en el estado $s$, se toma la acción $a$ y en lo subsiguiente se sigue la política $π$. Formalmente$$Q^\pi(s,a)=E_\pi\{R_t|s_t=s,a_t=a\}=E_\pi\{\sum_{k=0}^\infty\gamma^kr_{t+k+1}|s_t=s,a_t=a\}$$
***
La función de valor-acción óptima (denotada $Q^*$) se define como: $$Q^*(s,a)=\max\pi[Q^\pi(s,a)]$$
$Q^∗$ da el retorno esperado de tomar la acción $a$ en el estado $s$ y en lo sucesivo seguir una política óptima.