Una gramática regular es una 4-upla $(V,Σ,P,S)$ en donde:
- $N$ es el conjunto de símbolos no terminales
- $Σ$ es el conjunto de símbolos terminales [[Reglas Gramaticales#^6fb4ac|símbolos terminales]]
- $P$ Es el conjunto de *Producciones* que pueden ser de una de dos formas
	- $X\rightarrow aY$ con $X,Y∈N$ y $a∈\Sigma$
	- $X\rightarrow a$ con $X∈N$ y $a∈\Sigma$
	- Solo se permite $\lambda$ en la producción $S\rightarrow \lambda$ si $S$ no aparece en la parte derecha de alguna producción.
- $S$ es el símbolo inicial, llamado *símbolo distinguido*, perteneciente a los símbolos no terminales.
***
El [[Lenguajes Regulares|lenguaje]] generado por una gramática $G$, denotado $L(G)$, se define como$$L(G)=\{w∈Σ^*|S\dot⇒w\}\color{red}[1]$$
***
[[Derivación - Grámatica Regular]] 
[[Obtención de un AFD a partir de una Gramática Regular]] 
[1]. [[Clausura Reflexo Transitiva de la Derivación - Gramática Regular]] 