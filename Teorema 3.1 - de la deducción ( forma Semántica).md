Sean las fórmulas $P,Q$ y el conjunto $S \subseteq Form$. Entonces $$Q \in Con(S \cup\{P\})\leftrightarrow(P\rightarrow Q)\in Con(S)$$
***
($\Rightarrow$) $Q \in Con(S \cup\{P\})\rightarrow(P\rightarrow Q)\in Con(S)$
- Estrategia
	- Absurdo
- Supongamos que 
	- $Q\in Con(S\cup \{P\})$ 
	- $(P\rightarrow Q)\notin Con(S)$ 
- Entonces
	- Sea $v$ una [[Valuación que Satisface a una Fórmula|valuación]] que satisface a $S$.
		- Por definición de [[Consecuencia Lógica]], $v((P\rightarrow Q))=⊥$  
		- $v((P\rightarrow Q))=⊥$  si, y sólo si, $v(P)=\top \land v(Q)=⊥$ 
		- Por definición de valuación que satisface a una fórmula, lo anterior implica que 
			- $v$ satisface a $S\cup \{P\}$ 
			- $v$ no satisface a $Q$
		- Por definición de Consecuencia Lógica, esto significa que $Q\notin Con(S\cup \{P\})$ 
			- Lo último contradice nuestra hipótesis. 
			- Esto sucede por suponer que se puede tener que $Q\in Con(S\cup \{P\})$ y $(P\rightarrow Q)\notin Con(S)$.
			- Luego $Q \in Con(S \cup\{P\})\rightarrow(P\rightarrow Q)\in Con(S)$
($\Leftarrow$)$(P\rightarrow Q)\in Con(S)\rightarrow Q \in Con(S \cup\{P\})$
- Estrategia
	- Demostración Directa
- Supongamos que
	- $(P\rightarrow Q)\in Con(S)$ 
	- $v$ es una valuación que satisface a $S \cup\{P\}$
- Entonces
	- Sabiendo que $(P\rightarrow Q)≡(\neg P \lor Q)$  aseguramos que 
	- $v(P\rightarrow Q)=v(\neg P \lor Q)=v(\neg P) \lor v(Q)$ 
	- Sabiendo que $v(p_1 \lor ⊥)$ depende de $v(p_1)$, tenemos que
		- $v(Q)=⊥\lor v(Q)=\neg v(P) \lor v(Q)=v(P\rightarrow Q)=\top$ 
			- lo que muestra que $Q \in Con(S \cup\{P\})$

***
[[Corolario 3.1.1 del Teorema de la Deducción]] 