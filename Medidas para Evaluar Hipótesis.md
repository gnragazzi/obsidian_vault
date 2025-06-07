- Considerar la exactitud (accuracy) del modelo, 
	- porcentaje de aciertos de la hipótesis aprendida.
		- Si se deben categorizar objetos en n clases, corresponderá una matriz de confusión M de n × n.
		- ![[Pasted image 20250607134043.png]]
- Otras Medidas
	- Precisión ($\pi_{C}$)
		- La cantidad de objetos correctamente clasificados como C, sobre la cantidad total de objetos clasificados como C
	- Recall ($\rho_C$)
		- La cantidad de objetos correctamente clasificados como C, sobre la cantidad total de objetos C en la muestra
	- Normalmente se combinan estas 2 medidas para lograr la *F-Measure*
		- $F=\frac{2\pi\rho}{\pi+\rho}$ 
		- Caso particular de la función $F_\beta=\frac{(\beta²+1)\pi\rho}{\beta²\pi+\rho}$ con $\beta=1$.
	- ![[Pasted image 20250607134148.png]]
***
Consultar con la IA (si tengo ganas)
- Existen clases de modelos (por ejemplo, redes neuronales, k-NN, etc).
- Para utilizar un modelo en un proceso de entrenamiento, se elige una clase de modelo y se instancia
- Instanciar una clase de modelo es elegir una serie de valores para variables que tiene dicha clase de modelo y que se ajustan antes del entrenamiento 
	- Estos valores son llamados HiperParámetros y se diferencian de los parámetros, porque estos últimos se ajustan DURANTE el entrenamiento.
		- Ej Hiperparámetros #Preguntar_a_la_IA 
			- Para k-NN es, por ejemplo, k (cantidad de vecinos más cercanos)
		- Ej parámetros #Preguntar_a_la_IA 
![[Pasted image 20250607135233.png]]
![[Pasted image 20250607135240.png]]