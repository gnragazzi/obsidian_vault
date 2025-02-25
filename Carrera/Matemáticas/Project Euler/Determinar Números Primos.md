***
Versión 2
- Versión mejorada por la lectura del [[Características de los Números Primos|overview]].
- Manualmente pregunta si es múltiplo de 2 o de 3 (elimina la mayoría de números de entrada)
- Se establece directamente un límite superior adecuado
	- Al repecto de esto, debería decir, que me faltó un poco de análisis en la versión anterior: la idea era correcta (que no es necesario comprobar todos los números) pero tal vez la implementación no: porque claramente si el número es divisible por un número, el límite no importa; y si es primo el límite siempre se va a ir dividiendo hasta ese punto que es proporcional al número. Con un poco de análisis tal vez hubiese llegado a la idea que tal número es $sqrt(x)$
- Algo que no sabía: cada número primo puede ser expresado como 6k ± 1
```
def esPrimo(x):
    if(x==1):
        return False
    if(x==2 or x == 3):
        return True
    if(x%2==0 or x % 3 == 0):
        return False
    limite_superior= math.floor(math.sqrt(x))
    factor = 6 
    while(factor - 1 <= limite_superior):
        #print(f"Limite: {limite_superior}, factor: {factor}")
        if(x % (factor - 1)==0 or x % (factor + 1)==0):
            return False
        factor += 6
    return True
```
***
Versión 1
```
algoritmo esPrimo(x):Boolean
	divisor <- 2
	limite_superior <- x // divisor 
	mientras divisor <= limite_superior:
		if(x % divisor == 0):
			return False
		else:
			divisor += 1
			limite_superior= x//divisor
		 fi
	 finMientras
	return True
fin algoritmo
```

nota: // es división entera
***
[[Criba de Eratóstones]]