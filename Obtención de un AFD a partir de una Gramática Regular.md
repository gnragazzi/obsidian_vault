> [!Teorema]
>  *La clase de los lenguajes generados por alguna gramática regular es exactamente la de los lenguajes regulares*

Este teorema se prueba construyendo un [[Autómatas Finitos|Autómata Finito]] a partir de una [[Gramática Regular|gramática]] y visceversa.
Construir un autómata es directo: consiste en
- asociar a los [[Reglas Gramaticales|símbolos no términales]] de una gramática los estados del autómata.
	- Así, para cada regla $A→σB$ se da una transición $((A,σ),B)$ donde $A,B⊆Q$ y $σ∈E^*$
- El caso de reglas $A→b$, se tiene un nuevo estado$Z⊆F$ 
- Por último, $S=q_0$.
***
Para obtener una gramática a partir de un [[Autómata Finito Determinístico|AFD]] $D=(Q,Σ,δ,q_0,F)$, observamos que
- para cada transición de la forma $((p,σ),q)∈δ$ habrá en la gramática una regla $X_p→σX_q$ donde $X_i$ es la variable en la gramática que corresponde al estado $i$ del AFD. 
- La aplicación de reglas de la forma $X_p→σ$ se corresponden al consumo del último caracter de una palabra aceptada por el AFD. Por ello, para cada transición $((p,σ),q)∈δ$ donde $q∈F$, una regla adicional $X_p→σ$ se agrega.
***
![[Pasted image 20250405094231.png]]
![[Pasted image 20250405094238.png]]