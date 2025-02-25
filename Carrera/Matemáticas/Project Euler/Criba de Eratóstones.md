Es un algoritmo para encontrar los números primos menores a n
- Sea $n ∈ N$
- Sea $a[2..n]$ una lista de todos los números, de 2 a n
- Sea $p$ el número más chico de a sin ser tachado. Este número es primo. Si $p >= sqrt(n)$(\*¹), se termina el algoritmo
- - Sea $k ∈ N$. Todos los números pk en a son múltiplos de p, y por lo tanto no son primos. 
	- Tachamos todos los números pk <= n.
	- Podemos comenzar por los múltiplos a partir de p²(\*²)
- Volvemos al punto 3.
***
[10 - Overview | Project Euler]
***

\*¹. Esto se explica en (\*²)
\*². Sea p un número primo, y x un número tal que $p<x<p²$
	- Si x es primo, entonces no interesa dentro de la búsqueda de múltiplos
	- Si x no es primo pueden darse dos casos:
		- Que p no sea factor primo de x, en cuyo caso x no es múltiplo de p y no nos interesa
		- Que p sea factor primo de x, en cuyo caso $x=p*a1*..*an$, con a1..an el resto de los factores primos de x
			- Si $∀i ∈ [1..n]$ se cumple que $ai<p$, entonces x ya fue tachado en una iteración anterior del algoritmo.
			- Si $∃ai$ tal que $ai > p$, entonces $ai*p > p²$ y, por lo tanto, se puede comenzar la búsqueda de múltiplos a partir de $p²$