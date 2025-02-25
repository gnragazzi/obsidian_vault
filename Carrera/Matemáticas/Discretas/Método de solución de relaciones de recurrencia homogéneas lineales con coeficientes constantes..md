Sea $$a_n = c_1a_{n−1} + c_2a_{n−2}\ \ \ (1)$$
una [[Relación de recurrencia homogénea lineal con coeficientes constantes.|rrhl]] de segundo orden con coeficientes constantes. Entonces:
1. Si $S$ y $T$ son soluciones de (1), entonces$$U=bS+dT$$ con $b,d∈ℝ$ también es solución de (1). (Porque, por ejemplo, si $S$ soluciona $a_n$, con un coeficiente constante solucionaría $a_{n-1}$).
2. Si $r_1$ y $r_2$ son solución a la raiz $$t²-c_1t-c_2=0\ \ \ (2)$$entonces la sucesión $r_1^n$ y $r_2^n$ con $n=1,2,...$ son soluciones de 1.
3. Si 
	1. $a=a_1,a_2,...$ es la sucesión definida por (1), 
	2. $a_0=c_0 y a_1=c_1$
	3. $r_1$ y $r_2$ son soluciones a (2) y se tiene que $r_1≠r_2$
	entonces existen $b,d∈ℝ$ tales que $$a_n=br_1^n+dr_2^n$$ con $n=0,1,2,...$
4. Si todas las condiciones del punto anterior se cumplen, pero $r_1=r_2$, entonces$$a_n=br^n+ndr^n$$ con $n=0,1,2,...$
***
Ejemplo
Sucesión de Fibonacci
![[Pasted image 20250115130648.png]]