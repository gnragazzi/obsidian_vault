Sea $G = (N, \Sigma, P, S)$ una [[Gramáticas Libres del Contexto - GLC|gramática libre del contexto]], entonces puede construirse a partir de $G$ un [[Autómatas Push-Down - APD|APD]] [[Función de Transición Extendida - APD|extendido]] $M$ tal que $L(G) = L(M)$, donde:  
$$M = (\{p, q\}, \Sigma, N \cup \Sigma \cup \{\$ \}, \delta, q, \$, \{p\})  $$
y $\delta$ se construye como sigue:
1. $\delta(q, a, \lambda) = {(q, a)}$ con $a \in \Sigma$. Operación shift
2. Si $A \rightarrow \alpha \in P$, entonces $\delta(q, \lambda, \alpha)$ contiene a $(q, A)$
3. $\delta(q, \lambda, \$S) = {(p, \lambda)}$
***
Interpretación de cada regla
1. Incorpora el símbolo de la entrada a la pila para conformar las hojas de un posible subárbol del árbol total.
2. En la pila, una subcadena a partir del tope, es reconocida como un _handle_ o parte derecha de una producción y se reemplaza por su parte izquierda; es decir que se asciende en el Árbol de Derivación “conectando” los descendientes con el nodo padre.
3. El nodo raíz del Árbol de Derivación posiblemente ha sido alcanzado. Esto es, si la cadena a reconocer ha sido completamente analizada.
***
Dado que el tercer argumento de $\delta$ es una cadena de la pila y además estamos simulando una secuencia de derivaciones de más a la derecha, convendremos que el símbolo a la derecha de dicha cadena representa el tope de la pila. Una convención similar usaremos en las configuraciones.
***
#v2 