El problema se plantea como [[Problema - Agentes de Resolución de Problemas|los problemas de búsqueda estándar]] (con los 4 componentes). Los estados están definidos por los valores asignados hasta el momento.
- Estado Inicial: la asignación vacía, {}
- Función sucesor: asignar un valor a una variable no asignada
- Test de objetivo: la asignación actual es completa y cumple con las restricciones.
***
Particularidades de búsqueda estándar aplicada a PSRs
1. Es igual para todos los PSRs!
2. Cada solución aparece a profundidad $n$ con $n$ variables.
	1. Se usa la [[Búsqueda Primero en Profundidad]]
3. El paso es irrelevante (orden de asignación de valores)
4. $b=(n-l)d$ a prof. $l$, luego $n!d^n$ hojas y sólo hay $d^n$ asignaciones distintas! ^ae5cc8
	1. ¿Qué es $d$, en este caso? ¿Es la cardinalidad del dominio? ¿Que pasa si las variables tienen un dominio diferente? #Dudas 
	2. Ejemplo: ![[Captura de pantalla 2025-04-07 a la(s) 12.07.39 p. m..png]]
	3. Con respecto al punto anterior, observesé que las asignaciones son conmutativas (asignar primero un valor a $x$ y después un valor a $y$ es lo mismo que asignar primero un valor a $y$ y luego a $x$). Si aprovechamos esto, se tiene que
		1. ![[Captura de pantalla 2025-04-07 a la(s) 12.24.31 p. m..png]]
		2. Luego, $b=d$ y hay $d^n$ hojas
***
Tipos:
- [[Algoritmo Generar-y-Probar (Generate-and-Test)]]
- [[Algoritmos de Vuelta Atrás - Backtracking]]
