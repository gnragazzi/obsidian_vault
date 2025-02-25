```
función voraz(in C:conjunto): conjunto
{
	//C es el conjunto de candidatos
	s <- ∅ //construimos el conjunto solución en el conjunto S
	mientras C ≠ ∅
		x <- selección(C)
		C <- C - {x} // diferencia de conjuntos
		si factibilidad(S ∪ {x}) entonces S <- S ∪ {x}
	si solución(S) entonces
		devolver S
	sino
		devolver null
}
```
