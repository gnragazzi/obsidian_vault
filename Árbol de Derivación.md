Sea $G = (N, \Sigma, P, S)$ una [[Gramáticas Libres del Contexto - GLC|GLC]], luego un [[Árbol (Grafo)|árbol]] es un _Árbol de Derivación_ para $G$ si:
1. Cada nodo interior está rotulado por un símbolo no terminal.
2. Cada hoja es rotulada por un símbolo de $(N \cup \Sigma) \cup { \lambda }$. 
	1. No obstante si el nodo $n$ tiene rótulo $\lambda$, luego $n$ es una hoja y es el único descendiente de su padre. (Para las producciones del tipo $A \rightarrow \lambda$)
3. Si un nodo interior $n$ tiene rótulo $A$ y los vértices $n_1, n_2, \dots, n_k$ son los descendientes de $n$, de izquierda a derecha, con rótulos $X_1, X_2, \dots, X_k$ respectivamente, luego $A \rightarrow X_1 X_2 \dots X_k \in P$
![[Pasted image 20250504205547.png]]