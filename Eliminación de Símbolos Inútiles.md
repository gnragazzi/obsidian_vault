### Definición Formal

Si $G = \langle N, \Sigma, P, S \rangle$ es una GLC y $x \in (N \cup \Sigma)$, luego $x$ es un **símbolo útil** si existe una derivación $S \Rightarrow^* uxv \Rightarrow^* w$, donde $u, v \in (N \cup \Sigma)^*$ y $w \in \Sigma^*$. Un símbolo que no es *útil*, es llamado *inútil*.

*** 
### Interpretación

> De lo anterior, se puede decir que **un símbolo terminal es útil** si aparece en una cadena del lenguaje generado por $G$; **un símbolo no terminal es útil** si es **alcanzable**, es decir, si se encuentra al menos una ocurrencia de él en una secuencia de derivaciones que comienza desde el símbolo inicial y finaliza en una cadena de terminales.

### Algoritmos utilizados
- [[Construcción de una GLC libre de Símbolos Inútiles (Algoritmo 5)]]
- [[Construcción de una GLC donde todo no terminal deriva cadenas de terminales (Algoritmo 6)]]
- [[Construcción del conjunto de no terminales que derivan en  cadenas de terminales (A.7)]]
- [[Conjunto de no terminales alcanzables (Algoritmo 8)]]

***
#v2 