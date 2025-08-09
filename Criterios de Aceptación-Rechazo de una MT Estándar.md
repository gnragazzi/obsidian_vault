##### Aceptación:
- Si se llega a un estado final, la [[Máquina de Turing - Determinista|máquina]] se detiene y la cadena es aceptada
##### Rechazo
- Si $\delta(q_i,x_j)\text{ no está definida, con } q_i\subseteq Q, x_j\subseteq\Gamma$ entonces la máquina se detiene y la cadena es rechazada
- Si $\delta(q_i,x_j)=(q_k,x_k,I)$ y la MT está en la primera celda de la cinta, la máquina se detiene y la cadena es rechazada.
	- Se "cae" por izquierda

***
#### Etiquetas
#Anki 
