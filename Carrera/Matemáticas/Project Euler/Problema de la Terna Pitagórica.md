---
tags:
  - Dudas
  - Ejercicios
---
---
El problema es encontrar una terna $(a,b,c)$ tal que $a+b+c=s$, con $s∈N$
Si bien el problema es "sencillo" de resolver utilizando la fuerza bruta, encontré ***(Project Euler - Problema 9)*** la siguiente solución
***
- Si una terna pitagórica no es [[Terna Pitagórica Primitiva|primitiva]], entonces $∃ d ∈ N : MCD(a,b,c)=d$
- Luego, cualquier terna pitagórica o es primitiva o puede ser convertida en una dividiendo por su máximo común divisor:
$$
a²/d + b²/d = c²/d
$$
- De tal manera que cualquier terna pitagórica puede ser representada como una primitiva multiplicando cada uno de los términos primitivos por un d∈N:	
	(1)$$a = (m²-n²)d, b=2mnd, c=(m²+n²)d   $$
- de lo que se tiene que 
$$ a+b+c=d(m²-n²+2mn+m²+n²)=2m(m+n)d$$
	- De esto, tenemos que 
		 $s=2m(m+n)d$
-  Por lo que el problema se reduce a encontrar
	 - un $m>1$ que cumpla con $m|s/2$ (\*¹)
	 - un $k=(m+n)$ tal que $k | s/2m$ (\*²), que cumpla con que $m<k<2m$ (\*³). Por otro lado, k es impar (por definición, o m o n son impares)
	 - Además, se tiene que dar que MCD(m,k)=1 (\*⁴)
 - Si encontramos estos valores, determinar el valor de a, b y c se simplifica al proceso de reemplazar m, n y d en (1),
---
\*¹ Si $s=2m(m+n)d$, entonces  $s/2=m(m+n)d$. Luego, m es un divisor de s/2
\*² Del punto anterior, se deduce que Si $s/2=m(m+n)d$, entonces  $s/2m=(m+n)d$. Luego, m+n es un divisor de s/2m.
\*³ [[Terna Pitagórica Primitiva|Por definición]], $n > 0$, por lo que $m+n=k>m$, y $m>n$ por lo que $m+m=2m > m+n=k$
\*⁴ [[Terna Pitagórica Primitiva|Por definición]], $MCD(m,n)=1$. Si $MCD(m,k)=l$  entonces $k/l = (m+n)/l = m/l + n/l$, por lo que MCD(m,n)=l, algo que es contradictorio a la hipótesis por definición