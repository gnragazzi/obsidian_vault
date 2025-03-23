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
	- $((¬p_1∧¬p_2)→p_3$)
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
	- $((p_1∧p_2)→¬p_3)$
		- $p_1$ $x$ es un número racional
		- $p_2$ $y$ es un número entero
		- $p_3$ $z$ es un número real
- *9. Además de comer tarta, beberé sidra.*
	- ($p_1∧p_2$)
		- $p_1$ Comeré tarta
		- $p_2$ Beberé sidra
- *11. Si los gatos de mi hermana no soltaran tanto pelo me gustarı ́a acariciarlos.*
	- ($¬p_1→p_3$)
		- $p_1$ Los gatos de mi hermana sueltan pelo
		- $p_2$ Me gustaría acariciar a los gatos de mi hermana
- *13. Si mañana viene papá, o vamos al cine o vamos al circo con Josefa.*
	- $(p_1→(p_2∨p_3))$
		- $p_1$ $x$ Mañana viene papá
		- $p_2$ $y$ Mañana vamos al cine 
		- $p_3$ $z$ Mañana vamos al circo con Josefa
- 15. Para aprobar Lógica, el alumno debe asistir a clase(😅), desarrollar un cuaderno de prácticas aceptable y demostrar que dicho cuaderno ha sido desarrollado por él; o desarrollar un cuaderno de prácticas aceptable y aprobar el examen final.
	- $(((p_1∧p_2)∨(p_3∧p_4))→p_5)$
		- $p_1$ El alumno debe asistir a clase
		- $p_2$ El alumno debe desarrollar un cuaderno de prácticas aceptable
		- $p_3$ El alumno debe demostrar que dicho cuaderno ha sido desarrollado por él
		- $p_4$ El alumno debe aprobar el examen final
		- $p_5$ El alumno puede aprobar lógica
**
**Ejercicio 4**
Determinar cuáles de las siguientes secuencias pertenecen al lenguaje *Form* definido en teoría, justificando en cada caso su decisión. Cuando la razón sea la falta de paréntesis, transformarlas en fórmulas del lenguaje.  
- En base a la primera definición de fórmula vista el teoría, según la cual siendo $A^*$ el lenguaje referencial construido a partir del álfabeto $$A = \{ p, |, ¬, ∨, ∧, →, (, ) \}$$una lista de símbolos de A es una fórmula lógica si y solo si se la puede obtener aplicando un número finito de veces las siguientes reglas$^{(3)}$:
	1. Las [[Variables Proposicionales]] son fórmulas
	2. Si $P∈A*$ es una fórmula, entonces $¬P$ es una fórmula
	3. Si $P,Q∈A*$ es una fórmula, entonces $(P ∨ Q), (P ∧ Q) y (P → Q)$
	con esto en mente, observemos que 
- $1. ∨ p_0 ∉ Form$  
	- No se corresponde a una lista de símbolos de A que cumple las reglas descriptas en $^{(3)}$
	- El conectivo $∨$ debería ser binario en cualquier lista $∈Form$ 
- $3. ((p_3 ∨ ¬p_1) → p_2¬)$
	- No se corresponde a una lista de símbolos de A que cumple las reglas descriptas en $^{(3)}$
	- El conectivo $¬$ no antecede a una variable proposicional, como si lo haría en cualquier lista $∈ Form$
- $5. ¬((¬p_2 → p_3 ∧ p_4) ∨ p_1)$  
	- Para que sea una lista $∈Form$, la expresión $p_3 ∧ p_4$ debería estar entre paréntesis. 
	- La lista $¬((¬p_2 → (p_3 ∧ p_4)) ∨ p_1) ∈ Form$ 
- $7. (p_3 ∧ (p_1 → (¬p_2 ∨ p_3)) ∨ (p_4 → p_1))$ 
	- Faltan parentesis para que la lista considerada sea una fórmula lógica. Existen dos formas de agregar los paréntesis:
		- $((p_3 ∧ (p_1 → (¬p_2 ∨ p_3))) ∨ (p_4 → p_1))$ 
		- $(p_3 ∧ ((p_1 → (¬p_2 ∨ p_3)) ∨ (p_4 → p_1)))$ 
- $9. ¬(p_1 → (((¬p_2 → (p_3 ∨ (p_4 ∧ p_5))) → p_5) → ¬p_6))$
	- $¬(p_1 → (((¬p_2 → (p_3 ∨ (p_4 ∧ p_5))) → p_5) → ¬p_6))∈Form$. Teniendo en cuenta las reglas descriptas en $^{(3)}$:
		- $p_1$, $p_2$, $p_3$, $p_4$, $p_5$ y $p_6$ son fórmulas por 1.
		- $(p_4 ∧ p_5)$ es fórmula por 3.
		- $(p_3 ∨ (p_4 ∧ p_5))$ es fórmula por 3.
		- $¬p_2$ es fórmula por 2.
		- $(¬p_2 → (p_3 ∨ (p_4 ∧ p_5)))$ es fórmula por 3.
		- $((¬p_2 → (p_3 ∨ (p_4 ∧ p_5))) → p_5)$ es fórmula por 3.
		- $¬p_6$ es fórmula por 2.
		- $(((¬p_2 → (p_3 ∨ (p_4 ∧ p_5))) → p_5) → ¬p_6)$ es fórmula por 3.
		- $(p_1 → (((¬p_2 → (p_3 ∨ (p_4 ∧ p_5))) → p_5) → ¬p_6))$ es fórmula por 3.
		- $¬(p_1 → (((¬p_2 → (p_3 ∨ (p_4 ∧ p_5))) → p_5) → ¬p_6))$ es fórmnula por 2.
**
**Ejercicio 5**
Proporcionar expresiones del lenguaje castellano que puedan corresponder a las siguientes fórmulas, aclarando en cada caso qué proposición corresponde a cada variable proposicional:  
- $1. (p_1 → (p_2 ∧ p_3))$
	- $p_1$: Le compro a mi gato la comida que le gusta
	- $p_2$: Mi gato está contento
	- $p_3$: Mi gato se porta bien
	- "*Si le compro a mi gato la comida que le gusta, estará contento y se portará bien.*"
- $3. ¬(p_3 ∧ p_9)$
	- $p_3$: Hoy es miércoles
	- $p_9$: Hoy empieza el mes
	- '*No es cierto que hoy sea miércoles y empiece el mes.*'
- $5. (¬p_1 → ((p_2 → p_3) ∧ (p_3 → p_2)))$
	- $p_1$: Hoy tengo que trabajar
	- $p_2$: El día está lindo para pasear
	- $p_3$: Saldré a pasear
	- '*Si hoy no tengo que trabajar, entonces si el día está lindo, saldré a pasear y si salgo a pasear entonces el día está lindo*'
- $7. ((p_1 ∧ ¬p_3) ∨ (¬p_1 ∧ p_3))$
	- $p_1$: Estudio para el examen
	- $p_3$: Quedo libre en la materia
	- '*O bien estudio para el examen y no quedo libre en la materia, ó no estudio y quedo libre.*'
**
**Ejercicio 6**
Interprete las siguiente formas proposicionales utilizando, para cada variable proposicional, las expresiones listadas a continuación:  
$p_1$ = Andrés fue al dentista. 
$p_2$ = el dentista faltó a la cita. 
$p_3$ = el dentista le hizo un conducto a Andrés.
$p_4$ = el dentista tardó poco tiempo. 
p5 = los otros pacientes tuvieron que esperar. 

- $1. (p_1 ∧ ¬p_2)$
	- Andrés fue al dentista y este último no faltó a la cita.
- $3. ¬(p_1 ∧ p_4)$
	- No sucedió que Andrés fue al dentísta y el dentista tardó poco tiempo.
- $5. (¬p_1 ∧ ¬ p_4)$
	- Ni Andrés fue al dentista, ni el dentista tardó poco tiempo
- $7. (p_2 → (¬p_3 ∧ ¬p_5))$
	- El dentista no le hizo un conducto a Andrés y nos otros pacientes no tuvieron que esperar, dado que el dentista faltó a la cita.
**
**Ejercicio 7**
Dadas las siguientes fórmulas:  
- $i. ((p2 → ¬p3) → ¬(p2 ∧ (¬p5 → p3)))$
- $ii. (((¬(p1 ∧ p2) ∨ p2) → ¬p4) ∧ ¬p0)$
- $iii. (((¬(p1 → p1) ∨ p1) → ¬p4) ∨ ¬p1)$
1. Dar dos cadenas de formación irreducibles y dos que no lo sean, para cada una de ellas.  
2. En cada caso dar las secuencias de reglas (FP1), (FP2) y (FP3) utilizadas para escribir cada una de las fórmulas.
Recordamos que 
- Una cadena de formación de longitud $n$ es una sucesión finita $X_1, X_2, . . . , X_n$ de elementos de $A^∗$ que satisface las condiciones siguientes$^{(4)}$  
	- (CF) Para cada $i$, con $1 ≤ i ≤ n$, se tiene que:  
		- o bien $X_i$ es una variable proposicional, 
		- o bien existe un $j$ tal que 1 $≤ j ≤ i − 1$ y $X_i = ¬X_j$, 
		- o bien existen $j$ y $k$, ambos entre $1 ≤ j$, $k ≤ i − 1$, tales que
			- $X_i = (X_j ∨ X_k)$  o
			- $X_i = (X_j ∧ X_k)$ o 
			- $X_i = (X_j → X_k)$
- Una [[Cadena de Formación|cadena de formación]] $X_1, X_2, . . . , X_n$ se dice o *irreductible* si para todo $i$ tal que $1 ≤ i ≤ n − 1$, la sucesión $X_1, . . . , X_{i−1}, X_{i+1}, . . . , X_n$ no es una cadena de formación.

Por otro lado, *FP1*, *FP2* y *FP3* se corresponden a los puntos 1. 2. y 3. de $^{(3)}$
- $i. ((p2 → ¬p3) → ¬(p2 ∧ (¬p5 → p3)))$
	- 1.
		- [[Cadena de Formación|Cadenas de Formación]] [[Irreducibilidad - Cadenas de Formación|Irreductibles]] 
			- $$\matrix{
X_1 = p_2\\
X_2 = p_3\\
X_3 = p_5\\  
X_4 = ¬X_3\\  
X_5 = (X_4 → X_2)\\
X_6 = (X_1 ∧ X_5)\\  
X_7 = ¬X_6\\
X_8 = ¬X_2\\
X_9 = (X_1→X_8)\\
X_{10} = (X_9→X_6)
}$$
			- $$\matrix{
X_1 = p_2\\
X_2 = p_3\\
X_3 = ¬X_2\\
X_4 = (X_1→X_3)\\
X_5 = p_5\\  
X_6 = ¬X_5\\  
X_7 = (X_6 → X_2)\\
X_8 = (X_1 ∧ X_7)\\  
X_9 = ¬X_8\\
X_{10} = (X_4→X_9)
}$$
		- Cadenas de Formación no Irreductibles
			- $$\matrix{
X_1 = p_2\\
X_2 = p_3\\
X_3 = p_5\\  
X_4 = ¬X_3\\  
X_5 = (X_4 → X_2)\\
X_6 = (X_1 ∧ X_5)\\  
X_7 = ¬X_6\\
X_8 = ¬X_2\\
X_9 = (X_1→X_8)\\
X_{10} = ¬X_9\\ 
X_{11} = (X_9→X_6)
}$$
				- Observese que $X_1,X_2,...,X_9,X_{11}$ es una cadena de formación. Luego la anterior cadena de formación no es irreducible.
			- $$\matrix{
X_1 = p_2\\
X_2 = ¬X_1\\
X_3 = p_3\\
X_4 = ¬X_3\\
X_5 = (X_2∨X_4)\\
X_6 = (X_1→X_4)\\
X_7 = p_5\\  
X_8 = ¬X_7\\  
X_9 = (X_8 → X_3)\\
X_{10} = (X_1 ∧ X_9)\\  
X_{11} = ¬X_{10}\\
X_{12} = (X_6→X_11)
}$$
				- Observese que $X_1,X_2,...,X_4,X_6,X_7,...,X_{12}$ también es una cadena de formación. Luego la anterior cadena de formación no es irreducible.
	- 2.
		1. $p_2,p_3,p_5$ son fórmula por FP1.
		2. $¬p_5$ por FP2.
		3. $(¬p5 → p3)$ por FP3.
		4. $(p2 ∧ (¬p5 → p3))$ por FP3
		5. $¬(p2 ∧ (¬p5 → p3))$ por FP2
		6. $¬p_3$ por FP2
		7. $(p2 → ¬p3)$ por FP3
		8. $((p2 → ¬p3) → ¬(p2 ∧ (¬p5 → p3)))$ por FP3
- $iii. (((¬(p_1 → p_1) ∨ p_1) → ¬p_4) ∨ ¬p_1)$
	- 1.
		- [[Cadena de Formación|Cadenas de Formación]] [[Irreducibilidad - Cadenas de Formación|Irreductibles]] 
			- $$\matrix{
X_1 = p_1\\
X_2 = p_4\\
X_3 = ¬X_1\\  
X_4 = ¬X_2\\  
X_5 = (X_1 → X_1)\\
X_6 = ¬X_5\\  
X_7 = (X_6∨X_1)\\
X_8 = (X_7→X_4)\\
X_9 = (X_8∨X_3)\\
}$$
			- $$\matrix{
X_1 = p_1\\
X_2 = (X_1 → X_1)\\
X_3 = ¬X_2\\ 
X_4 = (X_3∨X_1)\\
X_5 = p_4\\
X_6 = ¬X_5\\  
X_7 = (X_4→X_6)\\
X_8 = ¬X_1\\  
X_9 = (X_7∨X_8)\\
}$$
		- Cadenas de Formación no Irreductibles
			- $$\matrix{
X_1 = p_1\\
X_2 = p_4\\
X_3 = ¬X_1\\  
X_4 = ¬X_2\\  
X_5 = (X_1 → X_1)\\
X_6 = ¬X_5\\  
X_7 = (X_6∨X_1)\\
X_8 = (X_7→X_4)\\
X_9 = (X_1∧X_2)\\
X_{10} = (X_8∨X_3)\\
}$$
				- Observese que $X_1,X_2,...,X_8,X_{10}$ es una cadena de formación. Luego la anterior cadena de formación no es irreducible.
			- $$\matrix{
X_1 = p_1\\
X_2 = (X_1 → X_1)\\
X_3 = ¬X_2\\ 
X_4 = (X_3∨X_1)\\
X_5 = p_4\\
X_6 = ¬X_5\\  
X_7 = (X_4→X_6)\\
X_8 = ¬X_1\\  
X_9 = (X_7∧X_8)\\
X_{10} = (X_7∨X_8)\\
}$$
				- Observese que $X_1,X_2,...,X_8,X_{10}$ es una cadena de formación. Luego la anterior cadena de formación no es irreducible.
	- 2. $(((¬(p_1 → p_1) ∨ p_1) → ¬p_4) ∨ ¬p_1)$
		1. $p_1$ es fórmula por FP1
		2. $(p_1 → p_1)$ es fórmula por FP3
		3. $¬(p_1 → p_1)$ es fórmula por FP2
		4. $(¬(p_1 → p_1) ∨ p_1)$ es fórmula por FP3
		5. $p_4$ es fórmula por FP1
		6. $¬p_4$ es fórmula por FP2
		7. $((¬(p_1 → p_1) ∨ p_1) → ¬p_4)$ es fórmula por FP3
		8. $¬p_1$ es fórmula por FP2
		9. $(((¬(p_1 → p_1) ∨ p_1) → ¬p_4) ∨ ¬p_1)$ es fórmula por FP3
**
**Ejercicio 8**
Decidir si las siguientes expresiones son fórmulas, utilizando el concepto de cadena de formación (expresado en $^{(4)}$).  
Recordamos que, según la segunda definición vista de fórmula lógica dice que una lista de símbiolos $P∈A*$ es una fórmula si y solo si existe una [[Cadena de Formación]] $X_1,X_2,...,X_n$ tal que $P=X_n$ .$^{(5)}$
- $1. ¬(p2 ∧ (¬p5 → p3))$
	- Sea $$\matrix{
X_1 = p_2\\
X_2 = p_3\\
X_3 = p_5\\ 
X_4 = ¬X_3\\
X_5 = (X_4→X_2)\\
X_6 = (X_1∧X_5)\\  
X_7 = ¬X_6\\
}$$ una cadena de formación de longitud 7. Observemos que $X_7=¬(p2 ∧ (¬p5 → p3))$. Por $^{(5)}$, $¬(p2 ∧ (¬p5 → p3))$ es fórmula.
- $3. ((p3 ∧ p2 ∨ p4 → p1)$
	- No es fórmula, puesto que no hay forma de construir una cadena de formación siguiendo los pasos descriptos en $^{(4)}$ (faltan paréntesis). 
- $5. (¬(p1 → p1) ∨ p1)$
	- sea $$\matrix{
X_1 = p_1\\
X_2 = (X_1→X_1)\\
X_3 = ¬X_2\\ 
X_4 = (X_3∨X_1)\\
}$$ una cadena de formación de longitud 4. Observemos que $X_4=5. (¬(p1 → p1) ∨ p1)$. Por $^{(5)}$, $5. (¬(p1 → p1) ∨ p1)$ es fórmula.
***
[1] https://www.rae.es/gtg/oraci%C3%B3n-de-modalidad-declarativa