Toma en cuenta [[Formulación Incremental - PSRs#^ae5cc8|esta idea]] y recorre el árbol usando algún algoritmo de búsqueda estándar (generalmente [[Búsqueda Primero en Profundidad]]) para asignar valores a las variables.
***
Es basicamente un ciclo que asina valores a todas las variables (Generar) y luego chequea si las mismas cumplen las restricciones (Probar).
```
Generar-y-Probar(): retorna una solución del PSR
Repetir
	asignaciones ← Generar(Variables, Dominios)
	Si probar(asignaciones)
		retornar asignaciones
```
***
Cada vez que es invocada, Generar(Variables,Dominios) retorna una asignación completa.
