#### Definición
Partiendo de la [[Construcción de MPCP a partir de <M,w>]], se tiene que $$\text{M acepta w ⇔ La instancia de MPCP construida tiene una solución}$$. La demostración involucra:
1. $\Rightarrow$
	1. Si $w\in L(M)$, entonces podemos comenzar con el par (1) y simular las computaciones de $M$ en $w$. 
		1. Usamos pares de la regla (3) para copiar el estado de cada configuración y simular un movimiento de M 
		2. Usamos pares de la regla (2) para copiar símbolos de cinta y el marcador $\#$ cuando se necesite
		3. Si M entra en $q_f$, entonces usamos los pares de las reglas 4 y 5, esta última para permitir que A "alcance" a B.
2. $\Leftarrow$ Si La instancia del MPCP construida tiene una solución, entonces M acepta w
	1. Cómo es una [[instancia MPCP]], todas las soluciones comienzan con.

| A    | B          |
| ---- | ---------- |
| $\#$ | $\#q_0w\#$ |
	2. Hasta que no se alcance $q_f$, no se utilizarán las reglas (4) ni (5). Por lo tanto, todos los estados (y cuando se agreguen símbolos) deberá ser manejados por las reglas (2) y (3). Es decir que, hasta que no se alcance el estado de aceptación, todas las soluciones tendrán la forma:

| A   | B    |
| --- | ---- |
| $x$ | $xy$ |
		donde x es la [[Secuencia de Configuraciones de una MT Determinística|secuencia de configuraciones]] de M, representando las computaciones de M en w, seguidas posiblemente por $\#$ y el comienzo de la siguiente configuración. $y$, por su lado es lo que queda de la configuración anterior, otro $\#$, y el comienzo de la próxima configuración
	3. Particularmente, entonces, si no se llega a un estado de aceptación, la secuencia de pares no es [[Solución MPCP|solución]] de la instancia, porque B siempre es más largo que A. Se sigue de esto que si hay una solución, es porque se llegó a un estado de aceptación; y $w\in L(M)$.
***
#### Etiquetas
- #Anki  

