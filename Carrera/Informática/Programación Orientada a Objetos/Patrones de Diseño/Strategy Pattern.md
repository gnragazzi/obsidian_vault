Definir una familia de algoritmos, encapsular cada uno y hacerlos intercambiables.
Permite variar el algoritmo independientemente del cliente que lo use.
***
![[Pasted image 20250210102314.png]]
***
- [[Principio de Diseño 8 - Principio Hollywood]]
	- Porque los clientes se comunican con la superclase, que a su vez se cumunican con las sub-clases y los comportamientos encapsulados, de manera que nunca hay una llamada de los componentes de bajo nivel a los de alto nivel
- 