#### Condición Simple $\sigma_{A=a}(r)$ 

- Si no hay índice en $A$
	- Costo Fuerza bruta 
- Si hay índice en A
	- Depende del índice
#### Condición Compuesta y conjuntiva $\sigma_{A=a\;AND\;B=b}(r)$ 

- Equivale a realizar las búsquedas de la condición simple por cada condición.
- Si hay un índice en alguna de las condiciones, 
	- se comienza por allí y luego se comprueba cada nupla de la relación resultante por cada condición
- Si hay un índice para las múltiples condiciones
	- Se utiliza ese índice
- En todos los casos, el costo depende de él/los índice/s.

#### Condición Compuesta y disyuntiva $\sigma_{A=a\;OR\;B=b}(r)$ 

- Si al menos un atributo no tiene índice
	- Costo fuerza bruta
- Si todos los atributos tienen índice
	- Depende del índice
***
#### Etiquetas
- #Anki 