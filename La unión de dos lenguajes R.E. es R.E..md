#### Definición
- Sean $L_1$ y $L_2$ dos lenguajes R.E. aceptados por $M_1$ y $M_2$.
- La [[La unión de dos lenguajes Recursivos es Recursivo|construcción similar para lenguajes recursivos]] no es válida para [[Lenguajes Recursivamente Enumerables|lenguajes R.E]].
	- Esto es porque en ese caso encadenamos la ejecución de $M_2$ a la respuesta NO de $M_1$ (que puede no llegar nunca si $L_1$ es R.E. en lugar de ser recursivo).
- Hipotetizo que la MT $M$ tal que $L(M)=L_1\cup L_2)$ a partir de $M_1$ y $M_2$ se construye de la siguiente manera:
	- M es una [[Máquina de Turing no Determinística - MTND]] que ejecuta $M_1$ y $M_2$ simultaneamente
	- Si alguna de las dos MTs acepta, M acepta
	- Si no rechazan, quedan en un loop de indecidibilidad (que está bien, pues es un lenguaje R.E.)
***
#### Etiquetas
- #Anki  