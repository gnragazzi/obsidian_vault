- Es [[Búsqueda Primero en Profundidad|búsqueda en profundidad]] limitada, aplicada iterativamente
- Es decir, primero prueba con $L=0$, si no encuentra solución, prueba con $L=1$, si no encuentra solución, con $L=2$, y así sucesivamente.
***
Evaluación
- Completa — Si 
- Tiempo
	- $(d+1)b^0+(d)b^1+(d-1)b^2+...+b^d=O(b^d)$
- Espacio
	- O(bd) 
- Óptima 
	- Si, con costos de paso idénticos.
***
```
función BÚSQUEDA-PROF-ITERATIVA(problema) retorna solución
	entradas: problema 
	para profundidad ← 0 hasta ∞ hacer
		resultado ← BUS-PROF-LIM(problema, profundidad)¹
		si resultado ≠ corte entonces retornar resultado
	finPara
finFunción 
```

***
![[Pasted image 20250329173121.png]]
![[Pasted image 20250329173158.png]]
![[Pasted image 20250329173206.png]]
***
¹. [[Búsqueda en Profundidad Limitada#^5f79ab|Algoritmo Búsqueda en Profundidad Limitada]]