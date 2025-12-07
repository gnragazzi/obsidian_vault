#### Definición Informal
- Dados dos problemas $A$ y $B$, ***reducir $A$ a $B$ significa***:  
	1. Transformar una instancia de $A$ en una instancia de $B$. 
	2. Resolver el problema $B$ para luego obtener la solución a $A$.
	usamos esta técnica para determinar que el problema $B$ es ***al menos tan dificil de resolver*** como el problema $A$. 
- En la práctica, esto significa que, en una reducción válida, 
	- Si el problema A no es [[Lenguajes Recursivos|recursivo]], el problema B tampoco lo es
	- Si el problema A no es [[Lenguajes Recursivamente Enumerables|R.E.]], el problema B tampoco lo es.
- Normalmente se reduce de un problema difícil conocido a un problema cuya dificultad se quiere demostrar
***
#### Definición Formal (¿Cuándo decimos que un problema A se reduce a un problema B?)

***Un problema $A$ reduce a un problema $B$***, si existe una función total  $$T : I_A → I_B$$ donde los conjuntos $I_A, I_B$ son el conjunto de instancias del problema $A$ y $B$, respectivamente.

![[Pasted image 20251128083427.png|400]]
- NOTAS SOBRE EL DIAGRAMA:
	- Una Reducción válida transforma las instancias SI del problema $A$ a instancias SI del problema $B$ (al igual que las instancias NO) y **no necesariamente** todas las instancias de $B$ tienen su correspondencia con instancias de $A$
***
#### Diagrama

![[Pasted image 20251128083133.png|500]]

***
#### Consecuencias de reducir un problema A (específico) a un problema B (versión más general)

- Si el problema A no es Recursivamente Enumerable, el problema B tampoco lo es
- Si el problema A no es [[Lenguajes Recursivos|recursivo]], el problema B tampoco lo es.
***
#### Etiquetas
- #Anki  