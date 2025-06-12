Sean $P , Q, R,S$ [[Fórmula Lógica|fórmulas]], y supongamos que $∗,◦$ representan a alguno de los conectivos $∨, ∧ o →$.  $$(P ∗ Q) = (R ◦ S)$$$$ →$$$$ P = R ∧Q = S ∧ ∗ = ◦.$$
***
Demostración
Lo haremos por el [[Demostración por Absurdo|absurdo]], 
- Sea $(P ∗ Q) = (R ◦ S)$ y que $P ≠ R$. En estas condiciones o bien 
	- $∃ X ∈ A^∗$ tal que $(R ◦ S) = (P ∗ X ◦ S)$ 
		- Tenemos que $R=P*X$
	- $∃  Y ∈ A^∗$ tal que $(P ∗ Q) = (R ◦ Y ∗ Q)$.  
		- Tenemos que $P = R ◦ Y$ . 
	- Pero por [[Carrera/Informática/23. Lógica para Computación/Lema 1#^f496f4|(ii)]] esto implicaría que $peso(P) > 0$ o $peso(R) > 0$, y ambas desigualdades son imposibles  ya que por hipótesis $R, P$ son [fórmulas] y por [[Carrera/Informática/23. Lógica para Computación/Lema 1#^d49e20|(i)]] su peso es cero.
Luego hemos probado que la igualdad $(P ∗ Q) = (R ◦ S)$ y$ P = R$.  De estas igualdades resulta inmediatamente que debe ser $∗ = ◦$ y $Q = S$, lo que concluye la demostración del teorema, c.q.d.