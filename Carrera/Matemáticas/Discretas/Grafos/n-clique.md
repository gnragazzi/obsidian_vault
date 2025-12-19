
Un n-clique en un grafo es un subgrafo con n nodos en el cuál cada par de nodos están conectados por un vértice.
El problema de decisión Asociado a un N-Clique es comprobar si un grafo tiene un n-clique. El lenguaje de decisión asociado al problema es$$CLIQUE=\{\langle G,k\rangle|\text{G es un grafo con un }n-clique\}$$

Un grafo con un 5-clique![[Pasted image 20251215212333.png|400]]

***
#### Transformación de 3-SAT a n-CLIQUE

Se puede [[Reducción en Tiempo Polinomial|transformar una instancia]] de [[Demostración de que 3-SAT es NP-Completo|3-sat]] con $k$ cláusulas en un Grafo de la siguiente manera:
1. Se representa cada cláusula como un grupo con 3 nodos llamado "triple"
2. Cada triple, que se corresponde a una cláusula, tiene cada uno de sus 3 nodos rotulados con los literales de la cláusula.
3. Se trazan vértices que unen todo par de nodos $n_1,n_2$, siempre que cumplan con las siguientes restricciones:
	1. $n_1,n_2$ pertenecen a distintos "triples"
	2. $n_1,n_2$ no se contradicen (por ejemplo, si el literal asociado a $n_1$ es x y el asociado a $n_2$ es $\neg x$, $n_1$ y $n_2$ se contradicen)
Por la construcción del n-Clique, observamos que: 
- si la instancia de 3-SAT tiene solución, entonces hay un literal en cada cláusula que es verdadero.
- Elegimos un nodo por cada cláusula que represente a literales verdaderos (tendremos al menos uno).
- El subgrafo compuesto por los nodos seleccionados y los vértices que los unen forman un k-clique.
La vuelta también es cierta: si existe un k-clique, entonces al los literales asociados a los nodos que lo forman se corresponden a literales (uno por cada clausula) que satisfacen a la fórmula.
Con respecto a la complejidad de la transformación, como la cantidad de nodos generados en el nuevo grafo es relativo a la cantidad de cláusulas (3k) y se generan, en el peor de los casos, k vértices por cada nodo, podemos ver que la complejidad temporal es polinomial, relativa al tamaño de la entrada.

***
#### CLIQUE ∈NP

Además, debería explicar que Clique es NP. Esto es casi trivial, pensando en una MTND que "adivina" k nodos. Luego, en la fase de verificación, por cada k-nodo seleccionado, se comprueba que hay un vértice entre este y el resto de los k-1 nodos. De esta forma, se obtuvo una MTND que resuelve este problema en tiempo polinomial no determinista.
***
#### Discretas

Un [[Grafo - Definición Formal|grafo]]/[[Digrafo - Definición Formal|digrafo]] [[Propiedades de Grafos#^0aa1c1|simple]] y [[Propiedades de Grafos#^e5f054|completo]] de [[Orden de un Grafo|orden]] n se denomina un ***n-clique***
Se denota $K_n$.

