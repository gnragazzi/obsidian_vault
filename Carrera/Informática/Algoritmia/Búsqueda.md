Computacionalmente, hablamos de buscar un elemento dentro de su estructura, hablamos de [[Evocación Asociativa]]. 
***
Los elementos que 
- se aportan en la búsqueda se denominan *Asociante* y se denotan $(*)$  
- se reciben en la búsqueda se denominan lo *Asociado* y denotan $(?)$ 
***
El problema de la búsqueda puede plantearse como 
> Tenemos una lista, L, de n elementos, y un elemento X.
> Tenemos que decidir si X∈L y, si lo está, apuntar al menos a una instancia de X en L.<

Si el [[Modelo]] aplicado a este problema es el [[Comparission_Based Model]], el algoritmo optimal es la [[Búsqueda Lineal]]
***
Si sabemos algo del orden de los elementos, podemos observar
- [[Jump Search - Algoritmo]]  ($∈O(\rceil\sqrt{n})$)
- [[Binary Search]]  ($∈O(\rfloor\ln{n}+1)$)