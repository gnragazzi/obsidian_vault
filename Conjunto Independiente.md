#### ¿Por qué el problema sobre grafos denominado Conjunto Independiente es NP? ¿cómo se prueba que es un problema N P-completo? Explique brevemente ambas preguntas.

Conjunto independiente es [[Clase de Lenguajes NP|NP]] porque existe una [[Máquina de Turing no Determinística - MTND|MTND]] que lo resuelve en [[Lenguaje Decidible en Tiempo Polinomial por MTND|tiempo polinomial]] no determinístico.
Funciona de la siguiente manera:
1. Se recibe una entrada $<G,k>$ con $G$ la representación de un [[Grafo - Definición Formal|grafo]] utilizando un conjunto de símbolos, y k un número entero que representa la cardinalidad del conjunto de nodos independientes.
2. Se eligen k nodos entre los nodos del grafo. Este es el paso no-determinístico, así que la MTND "adivina" un conjunto adecuado de nodos (de existir este conjunto)
3. Por cada uno de los k nodos, se comprueba que no estén relacionados con los k-1 nodos restantes.
La etapa de verificación (los últimos dos puntos) se repite k(k-1)/2 veces, por lo que su costo en términos de complejidad temporal es relativo a k² (polinomial relativo al tamaño de la entrada). Luego, Conjunto Independiente es NP.

Para probar que es [[NP-Completo|NP-Completo]], demostraremos que es [[Clase de Lenguajes NP-Duro (Completo)|NP-Duro]], logrando una reducción en tiempo polinomial desde un problema conocido como NP-Completo. Sea ese problema 3-SAT ((nota: acá me ahorro la explicación de 3-SAT que ya hice más arriba)). La reducción desde una Fórmula con k cláusulas es como sigue:
1. Se representa cada cláusula como un grupo con 3 nodos llamado "triple"
2. Cada triple, que se corresponde a una cláusula, tiene cada uno de sus 3 nodos rotulados con los literales de la cláusula.
3. Se trazan aristas que unen todo par de nodos $n_1,n_2$, siempre que cumplan con las siguientes restricciones:
    4. $n_1,n_2$ pertenecen al mismo "triple"
    5. $n_1,n_2$ se contradicen (por ejemplo, si el literal asociado a $n_1$ es x y el asociado a $n_2$ es $\neg x$, $n_1$ y $n_2$ se contradicen)
Luego, una instancia de 3-SAT transformada a un grafo tiene un conjunto independiente de tamaño k, formado por un nodo de cada "triple". Como los nodos independientes son de clausulas distintas, y los aristas unen únicamente nodos "contradictorios", si f es satisfacible, existe un conjunto independiente de k nodos.
Con respecto a la complejidad de la transformación, como la cantidad de nodos generados en el nuevo grafo es relativo a la cantidad de cláusulas (3k) y se generan, en el peor de los casos, 3k aristas por cada nodo, podemos ver que la complejidad temporal es polinomial, relativa al tamaño de la entrada.
Luego, podemos concluir que existe una reducción polinomial de 3-SAT a Conjunto Independiente. Concluimos, pues, que Conjunto independiente es (por propiedad transitiva) reducible desde cualquier Lenguaje Q en NP y, por lo tanto NP-Duro. Al ser NP y NP-Duro, concluimos que es NP-Completo.