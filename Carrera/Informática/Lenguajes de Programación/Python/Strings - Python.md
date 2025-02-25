- Cadenas de caracteres, envueltas tanto en '...', como en "..."
- Inmutables
***
Tipos
- Raw strings: Strings que no consideran caracteres escapados. Se consiguen anteponiendo una `r` al string.
```
	print('C:\some\name')  # here \n means newline! 
	print(r'C:\some\name')  # note the r before the quote
```
	
 - String Literals multilineas:
	 - Strings multi-linea.
	 - Sintaxis: `""" <string-literal> """` (triple comillas, simples o dobles)
	 - con \ se puede escapar el salto de linea. Útil para situaciones como 
```
	 print("""\ #NOTAR EL ESCAPE AL SALTO DE LINEA
Usage: thingy [OPTIONS]
     -h                        Display this usage message
     -H hostname               Hostname to connect to
""")
Usage: thingy [OPTIONS]
     -h                        Display this usage message
     -H hostname               Hostname to connect to
```

***
[[String - Python - Métodos]]