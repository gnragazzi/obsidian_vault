- Es el proceso de encontrar secuencias de acciones para llegar a un estado conocido (deseable o estado objetivo) y elegir la mejor, según alguna métrica. ^07cd3f
- El agente solo tiene un conjunto de acciones inmediatas.
- INFORMAL: *Cuando se habla de búsqueda, se habla de búsqueda de estados (del estado objetivo, digamos).*
***
Se realizan utilizando una estructura de datos llamada [[Árbol de Búsqueda - Búsqueda IA|Árbol de Búsqueda]] y aplicando una [[Estrategias de Búsqueda|Estratégia de Búsqueda]]
***
Proceso de la búsqueda: ^c92bac
1. Elegir un estado a explorar
2. Controlar si el estado es un estado objetivo
3. [Expandir el estado]^[1]
***
^[1] Generar el conjunto de estados que se obtienen de la aplicación de las acciones válidas en dicho estado. Se logra a través de la función EXPANDIR, que crea nuevos [[Nodo de Árbol de Búsqueda - IA|nodos]], completando los distintos campos y usando la función [[Problema - Agentes de Resolución de Problemas#^87763b|SUCESOR-FN]] del problema para crear los estados correspondientes.
***
[[Algoritmo de Búsqueda - IA]] 