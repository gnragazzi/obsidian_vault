$\infty_{LR}$ 
#### Definición
- Instancia: 
	- AFD $\langle M\rangle$
- Pregunta
	- $L(M)=\emptyset$
	- ![[Pasted image 20251105215350.png|400]]
#### Proceso 

![[Pasted image 20251105215851.png]]

1. Verificar si la instancia de entrada es correcta  
	1. Acotado por la longitud de la cadena $|<M>|$  
2. Determinar que acepta infinitas cadenas en $\Sigma^*$ 
	1. Deberían generarse cadenas hasta determinar que $M$ acepta infinitas cadenas.
	2. Por cada cadena $x$ determinar si pertenece a $x\in L(M)$

### Número de pasos acotados

Por el [[Lema de Pumping para Lenguajes Regulares (Teorema)|lema de pumping]] se sabe que generar cadenas hasta determinar que $M$ acepta infinitas cadenas está acotado por la cantidad de estados $|Q_M|\le|x|<2*|Q_M|$ 

![[Pasted image 20251105215703.png]]

***
#### Etiquetas
- #Anki 