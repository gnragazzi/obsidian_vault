Sea $G=<X,U,γ>$ un [[Digrafo - Definición Formal|digrafo]]/[[Grafo - Definición Formal|grafo]]
- Vertice Inicial - Final
	- Sea $u∈U$. Si $γ(u)=(x,y)$ con $x,y∈X$ el vértice $x$ es llamado el ***vértice inicial*** y el vértice $y$ es llamado ***vertice final*** del arco $u$.
- Sucesor/Predecesor
- Adyacencia
	- Dos vértices son adyacentes si están unidos por un arco/arista.
- Aislado
	- Si el [[Función de Grado Entrada,Saliente,Total|grado]] de un vértice, sacando bucles, es 0, se dice ***aislado***.
- Fuente
	- Un vértice se dice *fuente* si no tiene arcos entrantes.
- Sumidero
	- Un vértice se dice *sumidero* si no tiene arcos salientes.
- Raiz
	- $raiz(G)(x)⇔∀y∈X:\text{existe un camino¹ de x a y}$ ^0910a2
- Rais del grafo inverso
	- $raiz(G^{-1})(x)⇔∀y∈X:\text{existe un camino de y a x}$
***
¹. [[Camino]]
