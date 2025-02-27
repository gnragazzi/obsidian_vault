Computacionalmente, hablamos de buscar un elemento dentro de su estructura, hablamos de [[Evocación Asociativa]]. 
***
Los elementos que 
- se aportan en la búsqueda se denominan *Asociante* y se denotan $(*)$  
- se reciben en la búsqueda se denominan lo *Asociado* y denotan $(?)$ 
***
El problema de la búsqueda puede plantearse como 
> Tenemos una lista, L, de n elementos, y un elemento X.
> Tenemos que decidir si X∈L y, si lo está, apuntar al menos a una instancia de X en L.<

***
En este modelo lo que se cuenta como costo es el número de comparaciones.
***
Si el [[Modelo]] aplicado a este problema es el [[Comparission_Based Model]], y el algoritmo optimal es la [[Búsqueda Lineal]]
***
Si L está ordenada, tenemos otras opciones superadoras
- [[Jump Search - Algoritmo]]  ($∈O(\rceil\sqrt{n})$)
- [[Binary Search]]  ($∈O(\lfloor{\lg{n}}\rfloor+1)$)
***
$\lfloor{\lg{n}}\rfloor+1$ es optimal dentro del modelo de comparasión para cualquier [[Algoritmo Predecible (determinístico - estocástico)]]¹.
En este modelo, el algoritmo solo puede detenerse cuando encontró X o cuando agotó L (buscó en todos sus elementos).
***
¹. [Compared to what?]
