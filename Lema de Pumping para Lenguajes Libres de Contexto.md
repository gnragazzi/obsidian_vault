### Lema

Sea L un lenguaje libre de contexto. Entonces, existe un número $k$, que depende de $L$, tal que cualquier cadena $z\in L$ con $|z| \ge k$ pude ser escrita como $z=uvwxy$ donde:
1. $|vwx| \le k$
2. $|v|+|x|>0$
3. $\forall i \ge 0:uv^iwx^iy\in L$,
***
### Demostración

###### Idea

> Queremos demostrar que toda cadena de longitud mayor o igual a $k$ puede ser decompuesta de tal manera que cumpla el [Lema de Pumping], es decir que queremos probar 1, 2 y 3.

###### Condiciones

> Sea
>    - $L$ un [[Lenguajes Libres de Contexto - LLC|LLC]] 
>    - $G=\langle N,\Sigma,P,S\rangle$ una gramática que genera $L$, y se encuentra en [[Forma Normal de Chomsky - FNC|FNC]].
>    - $|N|=n$
>    - $k=2^n$
>    - $z\in L$ una cadena, con $|z|\ge k$

###### Demostración
###### Desarrollo general

1. Sea $S\Rightarrow^*z$ una derivación en $G$.
2. Por el [[Corolario 5.1 - Del Lema 5.1|corolario 5.1]], existe un [[Camino|camino]] de longitud al menos $n+1=|N| + 1$ en el [[Árbol de Derivación]] de $S\Rightarrow^*z$.
	1. Sea $p$ el camino de mayor longitud, desde la raiz hasta la hoja más profunda.
	2. $p$ debe contener _al menos_ $n+2$ nodos. Por el [[Principio del Palomar]], podemos asegurar que al menos un símbolo no terminal (diferente al símbolo distinguido, pues G está en FNC) que se repite alguna vez.
	3. Llamaremos a este no terminal que se repite, A.
3. El árbol de derivación de z puede ser dividido en 3 subárboles, donde los nodos etiquetados $A$ representan las últimas 2 ocurrencias de A en $p$.
	1.  ![[Pasted image 20250720122453.png]]

###### Prueba 3. $\forall i \ge 0:uv^iwx^iy\in L$
1. Las derivaciones en $z$ consisten en las siguientes sub-derivaciones
	1. $S\Rightarrow^*r_1Ar_2$
	2. $r_1\Rightarrow^*u$
	3. $A\Rightarrow^*vAx$
		1. Esta subderivación puede omitirse o repetirse un número arbitrario de veces antes de aplicar la derivación 4.
	4. $A\Rightarrow^*w$
	5. $r_2\Rightarrow^*y$
2. Estas derivaciones generan la cadena $z=uv^iwx^iy$ del lema.
###### Prueba 1. $|vwx| \le k$

1. El subcamino de p que representa $A\Rightarrow^*vwx$ será, a lo sumo, de longitud $n+2$. 
2. Luego, el árbol de derivación asociado tiene profundidad, a lo sumo $n+1$.
3. Por el [[Lema 5.1 - Sobre la longitud de una cadena en FNC|lema 5.1]]  podemos asegurar que $|vwx|\le 2^n=k$  
###### Prueba 2. $|v|+|x|>0$

1. La subderivación $A\Rightarrow^*vAx$ debe comenzar con una regla de tipo $A\rightarrow BC$, donde, ya B o ya C, derivan la ocurrencia A.
2. Asumamos que la derivación ocurre a partir de B. Entonces se tiene que
	1. $A\Rightarrow BC$
	2. $A\Rightarrow^* vAyC$, con $y\in \Sigma^*$
	3. $A\Rightarrow^* vAyz$, con $z\in \Sigma^*$
		1. es decir, existe una derivación $C\Rightarrow^* c$ que podemos asegurar no será nula, pues c deriva de una variable en una gramática en FNC.
	4. $A\Rightarrow^* vAx$, con $x=yz\in \Sigma^*$
3. Podemos afirmar que, dado que z no es una cadena vacía, x no será una cadena vacía.
4. Un análisis similar, demuestra que, si la segunda ocurrencia de A ocurre a partir de una derivación de C, entonces $|v|>0$, es decir, no es una cadena vacía
5. Luego, $|v|+|x|>0$


***
### Etiquetas
#v2 