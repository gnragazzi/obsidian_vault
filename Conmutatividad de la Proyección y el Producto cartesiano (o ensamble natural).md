#### Definición
- Si
	- $X = \{ A_1, A_2, \dots, A_n, B_1, B_2, \dots, B_m \}$
	- $A_1 A_2 \dots A_n$ son atributos de $r$  
	- $B_1 B_2 \dots B_m$ son atributos de $s$  
	-  en la condición $c$ sólo intervienen atributos de $X$
Entonces
$$
\pi_X \bigl( r \;\bowtie_c\; s \bigr) 
\;\equiv\; 
\bigl( \pi_{A_1 A_2 \dots A_n}(r) \bigr) 
\;\bowtie_c\; 
\bigl( \pi_{B_1 B_2 \dots B_m}(s) \bigr)
$$
- Si en la **condición $c$** intervienen atributos que no están en $X$, estos deben añadirse a $X$, por lo que se requiere una proyección final.  
- En el caso del producto cartesiano $\times$, no hay condición, por lo tanto la regla se aplica siempre.

***
#### Etiquetas
- #Anki 