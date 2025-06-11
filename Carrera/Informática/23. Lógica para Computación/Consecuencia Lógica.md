Sean $S\subseteq Form$ y $P\in Form$. 
Diremos que *$P$ es consecuencia de $S$* y escribiremos $S\models P$, en el caso que toda [[Función de Valuación|valuación]] $v$ que satisface a S también [[Valuación que Satisface a una Fórmula|satisface]] a P.
Esto es $$\forall Q \in S:v(Q)=\top \rightarrow v(P)=\top$$
***
Indicaremos con $Con(S)$ al conjunto de las consecuencias de $S$:$$Con(S)=\{P\in Form : S \models P\}$$
***
La [[Relación Binaria|relación]] de consecuencia es [[Transitividad|transitiva]].
***
Observaciones:
	- $Con(\emptyset)$ es el conjunto de todas las tautologías.   ^ea4f74
- a) Si $S=\emptyset$, entonces $P\in Con(S)$ si y solo si la fórmula $\neg P$ tiene un [[Árbol de Refutación]] [[Árbol de Refutación Cerrado - Abierto|cerrado]].
- b) Si $S=\{Q_1,...,Q_n\}$ entonces $P \in Con(S)$ si y sólo si la fórmula $(Q_1\land ...\land Q_n\land \neg P)$ tiene un árbol de refutación cerrado
***
[[Teorema 3.1 - de la deducción ( forma Semántica)]] 