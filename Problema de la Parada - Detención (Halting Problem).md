#### Definición
- El lenguaje asociado al ***Problema de la Detención***, $L_H$, es definido como $$L_H=\{<M,x> |\text{ MT M se detiene cuando se inicia con }x\;\}$$ este problema es no-decidible.
***
#### Demostración de la No Decidibilidad
1. Asumamos que el problema de la parada es [[Problemas Decidibles|decidible]]. Por lo tanto su lenguaje asociado, $L_H$ es [[Lenguajes Recursivos|recursivo]] y [[Lenguajes Recursivamente Enumerables|Recursivamente Enumerable]].
2. Como $L_H$ es R.E., entonces existe una [[Máquina de Turing Determinista - MT (MTD)|MT]] R tal que $L_H=L(R)$.
3. Construyamos una MT M' para decidir el problema asociado al [[Lenguaje Universal]], $L_U$ que funcione de la siguiente manera:
	1. Ante una entrada $<M,w>$, donde M es la [[Codificación de una MT usando {0,1}*|codificación binaria de una MT]] y $w$ una cadena binaria:
		1. Correr R con $<M,w>$ como entrada.
			1. Si R rechaza, M' rechaza.
			2. Si R acepta, continuar
		2. Simular $M$ con la entrada $w$ hasta que pare
			1. Si M acepta, M' acepta
			2. Si M rechaza, M' rechaza
4. Así, hemos construido una MT que siempre para y, por lo tanto, parecería que hemos probado que $L_U$ es recursivo y, por lo tanto, su problema asociado es decidible. Pero ya habíamos probado que $L_U$ [[Demostración de que LU no es recursivo utilizando Ld|no es un lenguaje recursivo]].
5. Esta contradicción se alcanza al asumir que el problema de la parada era decidible y que su lenguaje asociado es recursivo.
6. Por lo tanto, se concluye que el problema de la parada es no-decidible y su lenguaje asociado $L_H$ no es recursivo

***
#### Etiquetas
- #Anki  