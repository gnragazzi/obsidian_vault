Sea $S$ un subconjunto de $A^∗$ [[Cerrado por los Conectivos]]. Si $S$ contiene a todas las [[Variables Proposicionales]], entonces S contiene a todas las [[Fórmula Lógica|fórmulas]].
***
Importancia: 
El teorema anterior nos da un método para probar que las fórmulas tienen una determinada propiedad. Basta con tomar un conjunto $B ⊆ A^∗$, formado por todas las listas de símbolos que satisfacen una propiedad, digamos “propiedad-1”, y verificar que ese subconjunto de $A^∗$ es [cerrado por los conectivos] y contiene a todas las [variables proposicionales], para asegurar que todas las [fórmulas] están en $B$, por lo tanto todas las [fórmulas] satisfacen la propiedad “propiedad-1”. ^935052
***
Demostración (Por inducción)
Sea $S$ un subconjunto de $A^∗$ cerrado por los conectivos y que *contiene a todas las variables proposicionales*[(1)]. 
Queremos ver que para toda fórmula $P$ , se tiene que $P ∈ S$. 
Para ello razonaremos por inducción en la longitud de las cadenas de formación de $P$.  
- Supongamos primero que $P$ tiene una [[Cadena de Formación]] de longitud $n = 1$. 
	- Esto sólo es posible  si $P$ es una [variable proposicional], o sea que $P = p_k$ para algún número natural $k$, y en este caso $P ∈ S$ por hipótesis[(1)].  
- Sea $n > 1$. 
	- Como hipótesis inductiva suponemos que: para toda fórmula $Q$ que admita una cadena de formación de longitud < n, se tiene que $Q ∈ S$[(2)].
	- Supongamos que P admite una cadena de formación de longitud $n$, digamos $X_1, X_2, . . . , X_n$, con $X_n = P$. 
		- Si $X_n$ es una [variable proposicional], entonces ya sabemos que $P ∈ S$. 
		- Si no lo es, se pueden presentar los siguientes casos:  
			1. Existe $i$ tal que $1 ≤ i ≤ n − 1$ y $P = ¬X_i$ o  
			2. Existen $i, j$ tales que $1 ≤ i, j ≤ n − 1$ tales que $P = (X_i ∨ X_j), P = (X_i ∧ X_j) o P = (X_i → X_j)$.  
		- En el caso ***1***, $X_1, . . . , X_i$ es una cadena de formación de la fórmula $X_i$ de longitud $< n$.  
			- Luego, por la hipótesis inductiva[(2)], $X_i ∈ S$, y por ser $S$ cerrado por los conectivos cumple la propiedad $(C1)$, luego $P ∈ S$.  
		- En el caso ***2***, $X_1, . . . , X_i$ y $X_1, . . . , X_j$ son [cadenas de formación] de las [fórmulas] $X_i$ y $X_j$ respectivamente, ambas de longitud $< n$. 
			- Por la hipótesis inductiva $X_i ∈ S$ y $X_j ∈ S$[(2)], y por la propiedad (C2) de los conjuntos [cerrados por los conectivos] resulta que $P ∈ S$.  
Por el [[Principio de Inducción Matemática|principio de inducción]] resulta entonces que para todo número natural $n$, si la fórmula $P$ tiene una cadena de formación de longitud $n$, entonces $P ∈ S$.  Como toda fórmula tiene una [cadena de formación] de longitud finita, resulta que $Form ⊆ S$, c.q.d.