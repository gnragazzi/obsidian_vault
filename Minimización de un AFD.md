Es hallar un único AFD con la menor cantidad posible de estados.
***
Dado un AFD $M=(Q,Σ,δ,q_0,F)$:
1. [[Eliminar todos los estados que no pueden ser alcanzados desde el estado inicial]]
2. Utilizar el [[Algoritmo de Tabla Completa|algoritmo de tabla completa]] para encontrar todos los pares de estados equivalentes
3. Particionar Q en [[Construir bloques de estados|bloques de estados mutuamente equivalente]] 
4. [[Construir el AFD mínimo equivalente]] $N$, usando los bloques como sus estados.
***
