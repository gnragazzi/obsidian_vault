- `.` wildcard
	- todos los caracteres menos `\n`
- `[0-9]`
	- Rango desde el primer valor hasta el último, separado por un guión.
	- Una ocurrencia de cualquiera de los caracteres en el rango (en este ejemplo, cualquier número) hace match
	- Si se quiere incluir el símbolo `-` Se puede hacer usandolo al comienzo de los corchetes
		- `[-0-9]`, por ejemplo
- `a*` denota $\{λ, a, aa, aaa,...\}$
	- 0 o más ocurrencias
- `n+` denota $\{n , nn, nnn, nnnn,...\}$
	- 1 o más ocurrencias
- `a?` denota { λ, a}
	- 0 o 1 ocurrencia del caracter
- La Unión (|)
	- Opcional
	- `aaa | bbb | ccc` denota $\{aaa, bbb, ccc\}$
- Las llaves (`{ }`)
	- Sirven para usar E.R. Definidas anteriormente.
	- `pal [a-zA-`Z]+`
		- Luego se puede utilizar  `{pal}`  que es equivalente a `[a-zA-Z]+`
- `\` Escapa otro metasímbolo
- `^` 
	- Al principio de la linea
- `$`
	- Al final de la linea
***
Precedencia
![[Pasted image 20250402143236.png]]
***
![[Pasted image 20250402143422.png]]
***