#### Definición
- Una ***Planificación*** $P$ de $n$ transacciones $T_1,T_2,...,T_n$ es un ordenamiento de las operaciones de cada una de esas transacciones que cumple con la restricción de que, por cada transacción $T_i$ en $P$, las operaciones de $T_i$ en $P$ deben aparecer en el mismo orden en el que tienen lugar en $T_i$.

***
#### Notación
- Se utiliza
	- r -> leer
	- w -> escribir
	- c -> confirmar
	- a -> abortar
- identificador de la transacción
	- Subíndice en cada operación.
Ejemplo
![[Pasted image 20250905130836.png|200]]
***
#### Clasificación de las Planificaciones
1. [[Planificación en Serie|En serie]]
2. [[Planificación No-Serie|No-Serie]]
***
#### Propiedades
1. [[Serializable - Planificaciones|Serializable]]
2. [[Recuperabilidad]]
***
#### Etiquetas
- #falta 