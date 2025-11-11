>[! Todos los procesos involucrados en ∈LR deben finalizar en un número finito de pasos para que ∈LR sea un algoritmo y obtenga un resultado para cualquier cadena de entrada]
#### Definición
$\in_{LR}$ 
- Instancia: 
	- Un [[Autómata Finito Determinístico|AFD]] $M=\langle Q,\Sigma,\delta,q_0,F\rangle$ y una cadena $x\in\Sigma^*$ 
	- $I_{P_D}=\langle M,x\rangle\in\Sigma^*$ 
		- Esta última expresión indica que hay que [[Codificación de un AFD|codificar]] al AFD con los símbolos de $\Sigma$.
- Pregunta
	- $x\in\,L(M)$  
	![[Pasted image 20251105213814.png]]

#### Partes del problema:
- Verificar si la instancia del problema es correcta
- Ejecutar el AFD $M$ con la cadena de entrada $x$

![[Pasted image 20251105214348.png]]

Ambos procesos son acotados, por lo cual $\in_{LR}$ es un algoritmo.

***
#### Etiquetas
- #falta 