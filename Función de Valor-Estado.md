Denotaremos $V^π(s)$ al valor de un estado $s$ bajo una política $π$. Es decir, al retorno esperado cuando se comienza en el estado s y se sigue la política π. Formalmente $$V^\pi(s)=E_\pi\{R_t|s_t=s\}=E_\pi\{\sum_{k=0}^\infty\gamma^kr_{t+k+1}|s_t=s\}$$donde $E_π${} denota el valor esperado dado que el agente sigue la política $π$. Llamaremos a la función $V^π$ la ***función de valor-estado*** para la política $π$. 
***
La función valor-estado óptima es:
$$V^*(s)=\max_\pi[V^\pi(s)]$$
donde $\Pi$ es el espacio de todas las políticas posibles.
$V^∗$ indica para cada estado cual es el retorno esperado máximo que se puede obtener desde ese estado, sobre todas las políticas posibles, es decir cual es el retorno esperado que se obtiene siguiendo una política óptima