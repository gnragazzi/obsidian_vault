En grafos, una covertura de vértices es un subconjunto de los nodos de un grafo tal que todas las aristas del grafo tocan al menos un nodo de ese subconjunto. El problema pregunta si hay una covertura de vértices de tamaño k en un grafo G $$COB=\{<G,k> | G \text{ es un grafo que tiene una covertura de } k-vertices \}$$
Para probar que es [[NP-Completo|NP-Completo]], demostraremos que es [[Clase de Lenguajes NP-Duro (Completo)|NP-Duro]], logrando una reducción en tiempo polinomial desde un problema conocido como NP-Completo. Sea ese problema 3-SAT ((nota: acá me ahorro la explicación de 3-SAT que ya hice más arriba)). La reducción desde una Fórmula con m cláusulas es como sigue:
1. Se representa cada cláusula como un grupo con 3 nodos llamado "triple"
2. Cada variable se representa con 2 nodos, uno con su afirmación y uno con su negación.
3. Cada triple, que se corresponde a una cláusula, tiene cada uno de sus 3 nodos rotulados con los literales de la cláusula.
4. Las siguientes aristas
	1. Aristas que unen cada par de nodos en un mismo triple
	2. Aristas que unen las variables con su negación
	3. Aristas que unen las variables con sus representantes en los literales de las clausulas
  ![[Pasted image 20251216000148.png|400]]
