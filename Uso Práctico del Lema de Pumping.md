Dado que para todo [[Lenguajes Regulares|lenguaje regular]] infinito se cumple el [[Lema de Pumping para Lenguajes Regulares (Teorema)|lema de pumping]], si nos dan un [[Lenguaje - Definición|lenguaje]] infinito y demostramos que para él no se cumple, habremos demostrado que no es un lenguaje regular.
Cómo el lema es una propiedad que se cumple para todas las cadenas de longitud mayor o igual a cierto $n$, bastará encontrar una cadena de ese lenguaje, de longitud mayor o igual a esa $n$ que no se pueda *pump*ear para demostrar que el lenguaje no es regular.
Pasos para demostrar que un lenguaje dado NO es regular:
1. Asumir que el lenguaje dado es regular
2. Elegir una palabra $w$ que pertenezca al lenguaje, pero debe ser una cuya longitud sea $≥n$($n$ la constante del lema).
3. El lema dice que si el lenguaje fuera regular, podríamos encontrar una forma de subidividir $w$ en 3 subadenas $xyz$, cumpliendo las restricciones 1) y 2). Como queremos demostrar que el lenguaje no es regular, tendremos que demostrar que no hay ninguna forma de subdividir $w$, cumpliendo las restricciones del lema, y que después se pueda repetir (pumpear) $y$ en función del valor $k$ (la tercera condición del lema).
4. Bastará con encontrar una constante $k≥0$ que haga que ninguna de las particiones posibles de $w$ sea bombeable.
5. Por último, si para toda descomposición de la cadea se halló un $k$, que hace que cada una de las cadenas resultantes no pertenezca al lenguaje, concluimos que arribamos a una contradicción, que surge de haber asumido que el lenguaje era regular.
