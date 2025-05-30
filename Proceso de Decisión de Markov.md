![[Pasted image 20250511114829.png]]
- Extiende el [[Ambiente - Agentes#^8f2617|modelo de transición de estado determinístico]], permitiendo acciones probabilísticas cuyas consecuencias son perfectamente observables.
- En cada paso del tiempo $t$, el agente recibe como percepción una entrada $s_t$ y selecciona una acción $a_t$ aplicable al estado $s_t$
	- El tiempo es representado por una secuencia abstracta y discreta de pasos de tiempo $t = 0, 1, . . .$
	- Estos pasos no representan necesariamente intervalos fijos del tiempo real. Pueden referir a etapas sucesivas arbitrarias de toma de decisión y acción. 
- La acción generada por el agente cambia el estado del ambiente, el cual responde un paso del tiempo después con una indicación $s_{t+1}$ del nuevo estado del ambiente y una *señal de recompensa inmediata* $r_{t+1} ∈ \mathbb{R}$, por la acción tomada previamente.
	- ¿pensar r como el resultado de la [[Función de Utilidad]]? #Dudas 
- Con esto en mente, la tarea del agente se reduce a encontrar un comportamiento que le permita decidir en cada estado, qué acción tomar para maximizar los valores de la señal de recompensa acumulados a largo plazo
- Cuando el ambiente y la tarea satisface la [[Propiedad de Markov]], pueden ser definidas formalmente como un MDP que consiste de:
	- Un conjunto de estados posibles $S$
	- Un conjunto de acciones posibles $A$
	- Las dinámicas de un paso del ambiente, dadas por
		- Las probabilidades de transición $P(s,a,s')$ $$P(s,a,s')=Pr\{s_{t+1}=s'|s_t=s,a_t=a\}$$
			- Que debe leerse como la probabilidad de que el agente se encuentre en el estado $s′$ en el tiempo $t + 1$, si en el tiempo $t$ el agente ejecuta la acción $a$ en el estado $s$.
		- Las recompensas esperadas $R(s,a,s')$ $$R(s,a,s')=E\{r_{t+1}|s_t=s,a_t=a,s_{t+1}=s'\}$$
			- Lease como la recompensa esperada en el tiempo $t + 1$, si en el tiempo $t$, el agente realiza la acción $a$ en el estado $s$ y se produce la transición al estado $s′$ en el tiempo $t + 1$.
	- La solución a este MDP se reduce a encontrar una política óptima $\pi^*:S→A$ que en cada paso del tiempo $t$, en el estado $s_t$ elige la acción $a_t$ que maximiza el [[Retorno esperado en un MDP|retorno esperado]]. ^2a21ca
	- [[Enfoques para encontrar una solución a un MDP]]
	