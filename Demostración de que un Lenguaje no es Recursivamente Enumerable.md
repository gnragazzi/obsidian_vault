#### Demostración por el Método de la Diagonal de Cantor
1. Se supone que el conjunto (lenguaje) es enumerable 
2. Se realiza una secuencia, listando todos los elementos del conjunto $(x_1,x_2,x_3,...,x_n,...)$  
3. Se construye una matriz con la secuencia de elementos 
4. Se obtiene un nuevo elemento del conjunto, utilizando la diagonal de la matriz
5. Ese nuevo elemento debería estar dentro de la secuencia, pero no se lo encuentra porque difiere de todos los elemento en el listado
6. En conclusión, se obtiene una contradicción por suponer el listado exhaustivo de todos los elementos

***
#### Ejemplo
1. Supongamos que el conjunto $[0,1)$ es enumerable
2. Como dicho conjunto es enumerable, listaremos exhaustivamente todos sus elementos como $(x_1,x_2,x_3,...,x_n,...)$ donde cada $x_i=0,a_1a_2...$ donde cada $a_j\in \{0,9\}$
3. Construimos una matriz M donde cada entrada $m_{i,j}$ es el número $a_j$ del elemento $x_i$ del conjunto.
4. Sea $x=0,b_1b_2...$ un número tal que $\forall i \in \mathbb{N}: b_i \ne m_{i,i}$ 
5. Observemos que este $x\in [0,1)$ pero $\forall i\in\mathbb{N}:x\ne x_i$ pues difieren en el i-ésimo dígito decimal. Esto contradice que la lista fuese exhaustiva.
6. Por esta contradicción, se concluye que fue un absurdo suponer al conjunto como enumerable y es, por lo tanto, un conjunto infinito no-enumerable.

***
#### Etiquetas
- #Anki 