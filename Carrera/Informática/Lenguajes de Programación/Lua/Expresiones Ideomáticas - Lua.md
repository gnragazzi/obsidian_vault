
- Operador ternario: `<cond> and <resultado_si_verdadero> or <resultado_si_falso>`
	- ej: `mayor = (x>y) and x or y` (asigna a mayor el mayor valor entre x o y)
	- similar a = `mayor = x > y ? x : y`
	- [[Evaluación Perezosa]]
- `x = x or v`
	- Si x no tiene un valor, se le asigna el valor de v
	- if (not x) then x = v end