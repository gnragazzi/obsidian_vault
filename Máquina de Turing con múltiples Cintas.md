#### Definición
- Es una 6-upla $M=\langle Q,\Sigma,\Gamma,\delta,q_0,q_f\rangle$ como la MT Determinística
- Tiene $k$ cintas independientes (1 de entrada, $k-1$ cintas de trabajo) con $k$ cabezas lectograbadoras independientes
- La función de transición ahora es $$\delta:Q×\Gamma^k\rightarrow Q×(\Gamma×\{I,D,N\})^k$$es decir, debe registrar el estado de todas las cintas.
	- Ejemplo con 2 cintas
		- ![[Pasted image 20250817210306.png|500]]
***
#### Representación
![[Pasted image 20250817210519.png|400]]

#### Cómo se representan la transición de estados y la configuración en una de estas MT
![[Pasted image 20250920121436.png]]
![[Pasted image 20250920121341.png]]

***
#### Etiquetas
- #Anki 