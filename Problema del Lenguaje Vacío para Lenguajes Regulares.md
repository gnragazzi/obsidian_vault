$\emptyset_{LR}$ 
#### Definición
- Instancia: 
	- AFD M
- Pregunta
	- $L(M)=\emptyset$
	- ![[Pasted image 20251105214656.png]]

#### Proceso 
1. Verificar si la instancia de entrada es correcta  
	1. Acotado por la longitud de la cadena $|<M>|$  
2. Determinar que no existe ninguna cadena x en $\Sigma^*$ tal que $x \in L(M)$
	1. Deberían generarse cadenas hasta que:  
		1. En el proceso de evaluación de una cadena se alcance un estado final o
		2. Se hayan evaluado las suficientes cadenas para determinar que no es posible alcanzar ningún estado final desde el estado
		3. Por el [[Lema de Pumping para Lenguajes Regulares (Teorema)|lema de pumping]] se sabe que esto está acotado por la cantidad de estados $|x|<|Q_M|$ ![[Pasted image 20251105215030.png]]
		4. ![[Pasted image 20251105215212.png]]
***
#### Etiquetas
- #falta 