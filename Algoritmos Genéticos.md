- Analogía con la selección natural 
- Varios estados (población) van cambiando en cada iteración del algoritmo 
- Nuevos estados (sucesores) se obtienen ([[Crossover - Cruza|crossover o cruza]]) de la combinación de dos estados (padres)
- Cada estado es un individuo y es representado con un string de valores discretos (gralmente binario)
- La calidad de un individuo es medida con la *función de fitness* (mejor individuo, valor más alto de fitness)
- se introduce la "mutación" que produce cambios aleatorios en el "material genético", con probabilidad de mutación muy baja.![[Captura de pantalla 2025-04-07 a la(s) 5.53.04 p. m..png]]
***
Los individuos con mayor fitness tienen mayor probabilidad de tener copias en la próxima generación. Sea $P(t)=\{1,...,m\}$ la población en el tiempo t; y sea $f_i$ el fitness del individuo $i$ de $P(t)$. Entonces $$prob(i)=\frac{f_i}{\sum_{k=1}^mfk}$$
***
Algoritmo:
![[Captura de pantalla 2025-04-07 a la(s) 5.53.52 p. m..png]]
***
[[Mecanismos de Selección]]
***
Ejemplo
![[Captura de pantalla 2025-04-07 a la(s) 5.53.24 p. m..png]]