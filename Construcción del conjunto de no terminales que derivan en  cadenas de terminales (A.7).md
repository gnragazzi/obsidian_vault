
> Entrada: Una $GLC$ $G = ⟨N, Σ, P, S⟩$  
   Salida: El conjunto de no terminales que derivan en cadenas de terminales, $TERM$  
1. $TERM := \{A\space/\space \text{ hay una producción } A → w ∈ P \text{ con } w ∈ Σ^*\}$  
2. repetir  
	 1. $PREV := TERM$
	 2. Para cada no terminal $A ∈ N$ hacer
		 1. Si hay una producción $A → w$ y $w ∈ (PREV ∪ Σ)^*$ entonces
			 1. $TERM := TERM ∪ \{A\}$
	hasta $PREV = TERM$



#v2 