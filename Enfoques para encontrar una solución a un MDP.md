Si se dispone de las [[Función de Valor - MDP|funciones de valor]] óptimas $V^∗$ o $Q^∗$, $π^∗(s)$ puede ser derivada fácilmente desde las ecuaciones:			$$\pi^*(s)=arg \max_{a\in A(s)}[\sum_{s'\in S}P(s,a,s')[R(s,a,s')+\gamma V^*(s')]]$$o bien$$\pi(s)=arg\max_{a\in A(s)}[Q^*(s,a)]$$
***
Los enfoques para encontrar una solución a un MDP suelen diferir en alguno de los siguientes puntos:  ^8d6b82
- Aproximan $V^∗$ o $Q^∗$ como paso previo para derivar $π^∗$, o aproximan $π^∗$ directamente. 
- Cuentan o no con información sobre las dinámicas de un paso del ambiente (MDP’s con información completa vs MDP’s con información incompleta)
- La política óptima se obtiene antes de ser usada en el agente a ser controlado **(métodos off-line)**, o la política óptima es aprendida durante la fase de ejecución del agente, utilizando información que el agente acumula a medida que interactúa con el ambiente **(métodos on-line)**.  
- La actualización de las funciones de valor se basan en un **barrido exhaustivo** y sistemático del espacio de estados, o es posible actualizar sólo un subconjunto de estados, en instantes de tiempo posiblemente distintos (versión asíncrona).
***
- [[Value Iteration]]
- [[Q-Learning]]