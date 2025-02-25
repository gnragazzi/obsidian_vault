Sea $G$ un [[Grafo - Definición Formal|grafo]]/[[Digrafo - Definición Formal|digrafo]]. 
- $Trivial(G)≡|U|=0$ 
- $Regular(G) ≡ (∀x,y∈X) g(x)=g(y)$.[1] 
- $Simétrico(G) ≡ (∀u∈U):γ(u)=(x,y) ⇒ ∃u'∈U/γ(u')=(y,x)$ [2]
- $Completo(G)≡(∀x,y∈X):x≠y⇒|γ^{-1}(x,y)|+|γ^{-1}(y,x)|≥1$[3] ^e5f054
- $Simple(G)≡\text{si no tiene ni bucles ni arcos/aristas paralelas}$ ^0aa1c1
- $Conexo(G)≡ (∀x,y∈X) \text{ existe una cadena de x a y}$[4] ^797584
	- Si definimos la siguiente [[Relación Binaria|relación]] $$xE_Cy ⇔ \text{existe una cadena entre x e y }$$
		$E_C$ es una [[Relación de Equivalencia|relación de equivalencia]], que induce una [[Partición de un Conjunto|partición]] sobre el conjunto:  
		   - $P_{E_c}$: la partición inducida por $E_C$
	   Y caracterizar la propiedad de conexidad como $$\text{Un Grafo G es conexo} ⇔ |P_{E_C}|=1$$
	 - $Conexo(G)⇔$ admite un [[Grafo Parcial]] que sea [[Árbol (Grafo)|árbol]].
- $Fuertemente\ Conexo(G)≡ (∀x,y∈X) \text{ existe un camino de x a y}$[5] ^012695
	-  Si definimos la siguiente [[Relación Binaria|relación]] $$xE_{FC}y ⇔ \text{existe un camino entre x e y }$$
		$E_{FC}$ es una [[Relación de Equivalencia|relación de equivalencia]], que induce una [[Partición de un Conjunto|partición]] sobre el conjunto:  
		   - $P_{E_{FC}}$: la partición inducida por $E_{FC}$
	   Y caracterizar la propiedad de conexidad como $$\text{Un Grafo G es fuertemente conexo} ⇔ |P_{E_{FC}}|=1$$
***
[1]  [[Función de Grado Entrada,Saliente,Total]]
[2] Solo para [[p-digrafo|1-digrafo]]
[3]  [[Inversa de la Función de Incidencia|Inversa de función de incidencia]]
[4]  [[Cadena]]
[5]  [[Camino]]
