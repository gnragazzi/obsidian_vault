#### Definición Informal
- Dados dos problemas $A$ y $B$, ***reducir $A$ a $B$ significa***:  
	1. Transformar una instancia de $A$ en una instancia de $B$. 
	2. Resolver el problema $B$ para luego obtener la solución a $A$.

***
#### Definición Formal (¿Cuándo decimos que un problema A se reduce a un problema B?)

***Un problema $A$ reduce a un problema $B$***, si existe una función total  $$T : I_A → I_B$$ donde los conjuntos $I_A, I_B$ son el conjunto de instancias del problema $A$ y $B$, respectivamente.

![[Pasted image 20251128083427.png|400]]

***
#### Diagrama

![[Pasted image 20251128083133.png|500]]

***
#### Consecuencias de reducir un problema A (específico) a un problema B (versión más general)

- Si el problema A no es [[Recursivamente Enumerable]], el problema B tampoco lo es
- Si el problema A no es [[Lenguajes Recursivos|recursivo]], el problema B tampoco lo es.
***
#### Etiquetas
- #falta 