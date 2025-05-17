Sea $G = (N, \Sigma, P, S)$ una [[Gramáticas Libres del Contexto - GLC|gramática libre de contexto]], luego a partir de $G$ es posible construir un [[Autómatas Push-Down - APD|APD]] $M$ de manera tal que $L(G) = N(M)$; es decir un lenguaje aceptado por [[Lenguaje Aceptado por Pila Vacía|pila vacía]].  
La idea es construir $M$ de manera que pueda simular todas las derivaciones de más a la izquierda de $G$. De esta manera diseñamos al APD según la gramática $G$, como:
$$M = (\{q\}, \Sigma, \Sigma \cup N, \delta, q, S, \emptyset)$$
donde la [[Función de Transición - APD|función de transición]] $\delta$ se define como sigue:
1. Si $A \rightarrow \alpha \in P$, luego $\delta(q, \lambda, A)$ contiene $(q, \alpha)$. Operación **push**.
2. $\forall a \in \Sigma$, $\delta(q, a, a) = {(q, \lambda)}$. Operación **pop**.
***
1. En este caso, un movimiento independiente de la entrada, es decir, el símbolo corriente no es considerado. Porque lo que interesa es el tope de la pila, que representa el nodo de más a la izquierda en la frontera del árbol (parte abierta), siendo el candidato para la expansión. 
	1. El rango de la función $\delta$ representa las posibles alternativas para expandir dicho nodo 
		1. (posible no-determinismo dado que no tenemos información adicional para decidir por sólo una de ellas).
2. Si se alcanzó una hoja del árbol y coincide con la cadena de entrada, luego se elimina de la pila para continuar con la construcción del resto del árbol.