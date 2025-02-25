Es el más bajo del punto más alto del gráfico de uso de todos los algoritmos que resuelven el problema dentro del modelo.
***
Cómo, por [[Algoritmos|definición]], los algoritmos son secuencias finitas de operaciones, siempre habrá un mejor y peor costo.
***
Sean
- $M$ el modelo elegido
- $A_M$ el conjunto de todos los algoritmos que resuelven el problema dentro de $M$\*¹
- $I_n$ el conjunto de todas las entradas (inputs) posibles de tamaño $n$
- $f_A: I_n  → R⁺$ una función que mide el costo de recursos para el algoritmo A, dada una entrada de tamaño $n$.
Entonces:
$$Cota\ inferior\ para\ el\ peor\ costo\ de\ P=min_{[A∈A_M]}(max_{[I∈In]}(f_A(I)))$$
***
\*¹. Esto nos dice que lo que hacemos cuando elegimos un modelo es limitar el conjunto de algoritmos que resuelven el problema.
***
[Compared to what]