Se diferencia del [[Algoritmo Generar-y-Probar (Generate-and-Test)|Generate-and-Test]] porque este último sólo detecta violación de restricciones cuando se han realizado todas las asignaciones de valores a variables.
***
Este algoritmo es una [[Búsqueda Primero en Profundidad]] para PSRs con [[Estado del Problema#^57d29b|asignaciones consistentes]] (chequeamos las restricciones con cada asignación).
```
función Búsqueda-con-Vuelta-Atrás (psr) retorna solución/falla
retornar Vuelta-Atrás-Recursiva({},psr)

función Vuelta-Atrás-Recursiva(asignación,psr) return sln/fall
	si asignación es completa
		retornar asignación
	var ← SELECCIONA-VAR-NOASIGNADA(Variables[psr],asignación,psr)
	por cada valor en Ordena-Valores-Dominio(var,asignación,psr)
		si valor es consistente con asignación de acuerdo a Restricciones[psr]
			agregar{var=valor} a asignación
		resultado←Vuelta-Atrás-Recursiva(asignación,psr)
		si resultado ≠ falla entonces
			retornar resultado
		remover {var=valor} de asignación
		retornar falla
			
```
***
[[Mejoras a la Búsqueda con vuelta atrás]] 
