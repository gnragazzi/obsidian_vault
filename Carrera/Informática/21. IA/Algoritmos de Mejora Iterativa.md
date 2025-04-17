- Búsqueda local: mantener un único estado actual e intentar mejorarlo (moviendose a los vecinos) iterativamente![[Captura de pantalla 2025-04-07 a la(s) 5.27.26 p. m..png]]
```
función ASCENCIÓN-COLINA(problema) return un estado que es máximo local
entradas: problema
	local variables: actual, un nodo
					 vecino, un nodo
	actual ← HACER-NODO(ESTADO-INICIAL[problema])
	hacer ciclo
		vecino ← el sucesor de actual con el valor más alto
		si valor[vecino] ≤ valor[actual]
			return estado[actual]
		sino
			actual ← vecino
	fin
```
***
![[Captura de pantalla 2025-04-07 a la(s) 5.37.20 p. m..png]]
***
Solución: 
- [[Templado Simulado]] 
***
![[Captura de pantalla 2025-04-07 a la(s) 5.33.11 p. m..png]]![[Captura de pantalla 2025-04-07 a la(s) 5.33.19 p. m..png]]![[Captura de pantalla 2025-04-07 a la(s) 5.36.01 p. m..png]]