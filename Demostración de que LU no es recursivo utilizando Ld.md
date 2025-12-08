#### Demostración
- Se supone $L_U$, el [[Lenguaje Universal]], [[Lenguajes Recursivos|recursivo]].
- Por [[El Complemento de un Lenguaje Recursivo es Recursivo|teorema]] sabemos que su complemento, $\overline{L_U}$, definido como $$\overline{L_U}=\{\langle M,x\rangle|M \text{ es una máquina de Turing y x una cadena tal que }x\notin L(M)\;\}$$ es recursivo
	- Por lo tanto, al ser recursivo es [[Lenguajes Recursivamente Enumerables|recursivamente enumerable]] y [[MT como forma de demostrar que un lenguaje es o no R.E.|existe]] una [[Máquina de Turing Determinista - MT (MTD)|MT]] M tal que $L_U=L(M)$.
	- Esta MT realiza el siguiente procedimiento
		- Según su entrada $\langle MT,w\rangle$
		- Si $w\in L(MT)$, responde NO (no acepta la cadena)
		- Si $w\notin L(MT)$, responde SI (acepta la cadena)
- Pensemos en una nueva MT, M', que recibe una cadena binaria $x_i$ y realiza el siguiente procedimiento:
	- ![[Pasted image 20251130214415.png]]
	- Copia la cadena ingresada, logrando una codificación $<x_i,x_i>$.
	- Alimenta la MT que hipotéticamente resuelve $\overline{L_U}$. 
	- Si la MT $M_i$ (representada binariamente por la i-ésima cadena binaria (siguiendo el orden canónico), acepta a $x_i$ como entrada (se acepta a si misma), M' devuelve NO (no acepta la cadena).
	- Si $M_i$ no acepta $x_i$, responde SI (acepta la cadena).
- Observamos que $L(M')=L_d$. Pero $L_d$ ya fue probado no R.E.
	- Esta contradicción se alcanza por suponer $L_U$ como un lenguaje recursivo. 
- Luego, $L_U$ no es un lenguaje Recursivo.
***
#### Etiquetas
- #Anki  