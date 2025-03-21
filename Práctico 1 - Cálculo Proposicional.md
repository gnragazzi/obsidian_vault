**Ejercicio 1:**  
Analizar las siguientes frases y determinar cuáles son [[Proposición Lógica|proposiciones]], justificando su decisión en cada caso.
- *1. Las ballenas son mamíferos marinos.*
	-  Por definición, una proposición ***es una sentencia que es verdadera o falsa, pero no ambas*** caracterizada por ser una ***oración declarativa***, definida cómo aquella "*oración que expresa un juicio afirmando o negando algún estado de cosas*"[1]. Cómo corolario de esto, podemos decir que una proposición  ***no es interrogativa, ni exclamativa ni imperativa***.$^{(1)}$
	- Observamos que *Las Ballenas son mamíferos marinos* es una oración que afirma que el sujeto *Las Ballenas* cumple la propiedad *ser mamiferos marinos*.
	- Por $^{(1)}$, determinamos que *Las Ballenas son mamíferos marinos* es una proposición.
- *3. Todos los caballeros de la mesa redonda son leales a Arturo.*
	- Observamos que esta oración es nuevamente declarativa según la definición previa (afirma una propiedad de un sujeto, o en este caso, un grupo de sujetos).
	- Por $^{(1)}$, determinamos que la oración es una proposición.
- *5. Voy a comprar pan y a tomar un café.*
	- En este caso, la oración también es declarativa, afirmando 2 cosas que el sujeto que expresa la oración comunica que va a hacer.
	- Por $^{(1)}$, determinamos que la oración es una proposición, aunque en este caso una compuesta de dos proposiciones simples: *Voy a comprar pan*, *Voy a comprar café* unidas por una [[Conjunción|conjunción]].
- *7. Cierra la puerta.*
	- En este caso, vemos que la oración es imperativa: ordena a alguien que haga algo
	- Por $^{(1)}$, determinamos que esta oración no es una proposición.
- *9. ¡Me duele!*
	- Observamos que esta es una oración exclamativa, por lo que, por $^{(1)}$, determinamos que no es una proposición
- *11. ¿Juan es el maestro de Paola?  *
	- Esta oración, que claramente es interrogativa, tampoco es una proposición, según lo definido en $^{(1)}$.
- *13. π por radio al cuadrado es igual a la superficie del círculo.*
	- Esta oración es declarativa, al determinar la igualdad entre *π por radio al cuadrado* y *la superficie del círculo*. Esta igualdad será cierta o no y, por lo expresado en $^{(1)}$, determinamos que es una proposición.
**
**Ejercicio 2:**
Sea $L_1$ el lenguaje obtenido a partir del alfabeto $A_1 = \{∗, ∼, ▷◁\}$ y la siguiente gramática$^{(2)}$:
1. $▷◁$ es una fórmula; $∼ ▷◁$ es una fórmula.  
2. Si X es una fórmula, entonces  
	1. $∼ X$ también lo es.  
	2. $▷◁ ∼ ∗ X$ también lo es.  
	3. $∼ ∗ X$ también lo es.  
3. $X$ es una fórmula si y sólo si se la puede obtener aplicando un número finito de veces las reglas anteriores (condición última).
- 1. Para cada una de las siguientes secuencias decidir si son o no fórmulas del lenguaje $L_1$:
	- a) $∗$
		- No lo es, pues no se puede llegar a ella siguiendo $^{(2)}$.
	- c) $∼$
		- No lo es, pues no se puede llegar a ella siguiendo $^{(2)}$.
	- e) $∼∼ ∗ ▷◁$
		- Si lo es pues se puede construir siguiendo las siguientes reglas de $^{(2)}$ 
			- $▷◁$ es una fórmula (por 1)
			- $∼ ∗ ▷◁$ es una fórmula (por 2.3)
			- $∼∼ ∗ ▷◁$ es una fórmula (por 1)
	- g) $▷◁ ∼ ∗ ∼∼ ∗ ∼$
		- No lo es, pues no se puede llegar a ella siguiendo $^{(2)}$.
	- i) $∼ ∗ ∼ ▷◁$
		- Si lo es pues se puede construir siguiendo las siguientes reglas de $^{(2)}$ 
			- $∼ ▷◁$ es una fórmula (por 1)
			- $∼ ∗ ∼ ▷◁$ es una fórmula (por 2.3)
- 2. Escribir 5 expresiones de $L_1$ que no sean fórmulas y 5 que si lo sean. En cada caso, cuando sea fórmula, mostrar la secuencia de reglas de la gramática que aplicó para obtenerlas.
	- Expresiones de $L_1$ que no son fórmulas
		- $∗ ▷◁$
		- $∼$
		- $▷◁▷◁$
	- Expresiones de $L_1$ que sí son fórmulas, según $^{(2)}$
		- $∼∼▷◁$
			- $∼▷◁$ es fórmula (por 1)
			- $∼∼▷◁$ es fórmula (por 2.1)
		- $▷◁ ∼ ∗ ∼▷◁$
			- $∼▷◁$ es fórmula (por 1)
			- $▷◁ ∼ ∗ ∼▷◁$ es fórmula (2.2)
		- $▷◁ ∼ ∗ ∼ ▷◁ ∼ ∗ ∼▷◁$
			- $▷◁ ∼ ∗ ∼▷◁$ es fórmula (demostrado en el punto anterior)
			- $∼ ▷◁ ∼ ∗ ∼▷◁$ es fórmula (por 2.1)
			- $▷◁ ∼ ∗ ∼ ▷◁ ∼ ∗ ∼▷◁$ es fórmula (por 2.2)
**
**Ejercicio 3:** 
Representar las siguientes expresiones del lenguaje natural en forma simbólica, utilizando los símbolos de la lógica proposicional y explicitando claramente las proposiciones simples que intervienen ($p_1, p_2, p_3$, etc.). 
- *1. A Pedro no le gusta el dulce de leche ni la miel.*
	- $¬(p_1∧p_2)$ 
		- $p_1$ "A pedro le gusta el dulce de leche"
		- $p_2$ "A pedro le gusta la miel"
- *3. Si no hay ruidos y no estás sordo, entonces debes oírme.*
	- $(¬p_1∧¬p_2)→p_3$
		- Si bien la expresión no es ambigua dada la precedencia de operadores, optamos por el uso de paréntesis por claridad.
		- $p_1$ Hay ruido
		- $p_2$ Estás sordo
		- $p_3$ Debés oirme
- *5. Prefiero ir de vacaciones o estar sin hacer nada si tengo tiempo para ello y no tengo que ir a trabajar.*
	- $(p_3∧¬p_4)→(p_1∨p_2)$
		- $p_1$ Prefiero ir de vacaciones
		- $p_2$ Prefiero estar sin hacer nada
		- $p_3$ tengo tiempo
		- $p_4$ tengo que ir a trabajar
- *7. Si $x$ es número racional e $y$ es un número entero, entonces $z$ no es real.*
	- $(p_1∧p_2)→¬p_3$
		- $p_1$ $x$ es un número racional
		- $p_2$ $y$ es un número entero
		- $p_3$ $z$ es un número real
- *9. Además de comer tarta, beberé sidra.*
	- $p_1∧p_2$
		- $p_1$ Comeré tarta
		- $p_2$ Beberé sidra
- *11. Si los gatos de mi hermana no soltaran tanto pelo me gustarı ́a acariciarlos.*
	- $¬p_1→p_3$
		- $p_1$ Los gatos de mi hermana sueltan pelo
		- $p_2$ Me gustaría acariciar a los gatos de mi hermana
- *13. Si mañana viene papá, o vamos al cine o vamos al circo con Josefa.*
	- $p_1→(p_2∨p_3)$
		- $p_1$ $x$ Mañana viene papá
		- $p_2$ $y$ Mañana vamos al cine 
		- $p_3$ $z$ Mañana vamos al circo con Josefa
- 15. Para aprobar Lógica, el alumno debe asistir a clase(😅), desarrollar un cuaderno de prácticas aceptable y demostrar que dicho cuaderno ha sido desarrollado por él; o desarrollar un cuaderno de prácticas aceptable y aprobar el examen final.
	- $((p_1∧p_2)∨(p_3∧p_4))→p_5$
		- $p_1$ El alumno debe asistir a clase
		- $p_2$ El alumno debe desarrollar un cuaderno de prácticas aceptable
		- $p_3$ El alumno debe demostrar que dicho cuaderno ha sido desarrollado por él
		- $p_4$ El alumno debe aprobar el examen final
		- $p_5$ El alumno puede aprobar lógica
	 

***
[1] https://www.rae.es/gtg/oraci%C3%B3n-de-modalidad-declarativa