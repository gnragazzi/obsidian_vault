Para toda [[Fórmula Lógica|fórmula]] $P$ se tiene que:
- (i) $comp(P ) = 0 ⇔ P\text{ es una variable proposicional}$.  
- (ii) Si $comp(P ) > 0$, entonces se cumple uno y sólo uno de los casos siguientes:  
	1. Existe una única fórmula $Q$ tal que $P = ¬Q$.  
	2. Existe un único par de fórmulas $Q, R$ tal que $P = (Q ∨ R)$.  
	3. Existe un único par de fórmulas $Q, R$ tal que $P = (Q ∧ R)$.  
	4. Existe un único par de fórmulas $Q, R$ tal que P = $(Q → R)$.
***
***Demostración:***
La parte (i) del enunciado es obvia ya que las variables proposicionales no incluyen conectivos. 
La parte (ii) es una consecuencia inmediata de la definición de [fórmula] y del [[Teorema 2 - Unicidad de la Lectura de las Fórmulas]].