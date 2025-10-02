#### Objetivo
- Producir una [[Equivalencia de Expresiones del Álgebra Relacional|consulta equivalente]] a la dada pero cuya ejecución sea más eficiente que la original.
- Mejora el costo de evaluar la consulta independientemente de la estructura física de los datos (índices).
- Usada para optimizar la representación interna inicial (uso de heurísticas)
***
#### Reglas
1. [[Cascada de Selecciones]]
2. [[Conmutatividad de la Selección]]
3. [[Cascada de Proyecciones]]
4. [[Conmutatividad de Proyección y Selección]]
5. [[Conmutatividad del Ensamble y el Producto Cartesiano]]
6. [[Conmutatividad de la Selección y el Producto cartesiano (o ensamble natural)]]
7. [[Conmutatividad de la Proyección y el Producto cartesiano (o ensamble natural)]]
8. [[Conmutatividad de Operaciones de Conjunto]]
9. [[Asociatividad de Operaciones]]
10. [[Conmutatividad de Selección con operaciones de conjunto]]
11. [[La proyección se conmuta con la unión]]
12. [[Conversión de una secuencia σ, X en ensamble natural con selección]]

#### Principios de la Manipulación Algebraica
1. Realizar las selecciones tan pronto como sea posible.  
2. Si existe un producto cartesiano seguido de una selección, combinarlos para producir un $\bowtie$   
3. Combinar secuencias de operaciones unarias.
4. Buscar subexpresiones comunes en una expresión.
***
#### Etiquetas
- #Anki 