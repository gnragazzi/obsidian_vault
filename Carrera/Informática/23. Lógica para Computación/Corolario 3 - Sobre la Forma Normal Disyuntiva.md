Toda [[Fórmula Lógica|fórmula]] que no sea [[Tautología, Contradicción y Contingencia#^476267|contradicción]] es [[Equivalencia de Fórmulas Lógicas|lógicamente equivalente]] a una fórmula restringida de la forma $$\left( \bigvee_{i=1}^{m} \left( \bigwedge_{j=1}^{n} Q_{ij} \right) \right)$$
siendo $Q_{i,j}$ una variable proposicional o la negación de una variable proposicional. Esta forma se llama ***forma normal disyuntiva***.
***
$n$ se corresponde con la cantidad de variables de la función y $m$ con la cantidad de valuaciones (filas) que hacen a la fórmula verdadera.
***
EJEMPLO: 
Sea una función de verdad especificada a través de la siguiente tabla (se trata de una función de tres argumentos):
![[Pasted image 20250523212800.png]]
Las combinaciones de valores de verdad para las que la función arroja el valor $\top$ son:  
$\top\ \top\ \top$, $\top\ \top\ \bot$ y $\bot\ \bot\ \bot$ (fila 1, fila 2 y fila 8), por lo tanto las conjunciones básicas correspondientes son:$$(p_1 \land p_2 \land p_3) $$$$ (p_1 \land p_2 \land \neg p_3) $$$$ (\neg p_1 \land \neg p_2 \land \neg p_3)$$La fórmula construida siguiendo la demostración es:
$$(p_1 \land p_2 \land p_3) \lor (p_1 \land p_2 \land \neg p_3) \lor (\neg p_1 \land \neg p_2 \land \neg p_3)$$
Esta fórmula corresponde a la función de verdad dada y su tabla de verdad coincide con la tabla dada.
***
![[Captura de pantalla 2025-03-31 a la(s) 4.08.26 p. m..png]]
***