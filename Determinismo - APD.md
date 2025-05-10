Un [[Autómatas Push-Down - APD|APD]] será deterministico si su función de transición cumple las siguientes restricciones:
- $\forall q \in Q \land Z \in \Gamma$ siempre que $\delta(q, \lambda, Z)$ esté definida, luego $\delta(q, a, Z)$ está indefinida $\forall a \in \Sigma$. 
	- No permite simultáneamente movimientos independientes y dependientes de la entrada para un mismo $q$ y $Z$.    
- Para ningún $q \in Q$, $Z \in \Gamma$, $a \in (\Sigma \cup { \lambda })$; $\delta(q, a, Z)$ no contiene más de un elemento. 
	- **La cardinalidad del conjunto de posibles acciones puede ser uno o cero.**
***
La familia de [[Lenguaje - Definición|lenguajes]] reconocidos por APD-no determinísticos no es equivalente a la reconocida por APD-deterministicos. En particuar se cumple que:$$APD_{\text{deterministicos}}\subset APD_{\text{no-deterministicos}}$$
