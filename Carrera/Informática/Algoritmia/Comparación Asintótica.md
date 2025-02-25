Consiste en comparar la [[Tasa de Crecimiento]] de dos funciones, de manera de saber si una crece más rápidamente que la otra, a partir de un cierto valor de $n$. 
Este costo es importante porque a veces es muy complejo (o costoso) saber el costo exacto de un [[Algoritmos|algoritmo]], así que comparamos su función de costo con funciones más simples, cuya tasa de crecimiento es conocida, utilizando [[Notación O]].
***
La comparación, notación y análisis asintóticos nos hablan de lo que pasan cuando $n→∞$, es decir, de cuando las entradas son exageradamente grandes (más grandes de lo que encontraríamos en una situación práctica) a partir de un punto. 
Esto puede parecer indicar que, como no nos habla *necesariamente* del desempeño de un algoritmo en el rango de lo práctico, no es importante.
Sin embargo, la [[Tasa de Crecimiento|tasa de crecimiento]] de los costos de un algoritmo pueden decirnos algo sobre como se comporta el algoritmo cuando las entradas son *razonablemente* grandes.