#### Definición
- Dada la [[Dependencia Multivaluada|dmv]] $X\rightarrow\rightarrow Y$ en R, descomponemos en dos subesquemas: $$R_1=X\cup Y\text{ y }R_2=R-Y$$y se asegura la descomposición sin pérdida de información.
***
#### Nota
Cualquiera de las siguientes es condición suficiente y necesaria:
- $R_1∩R_2\rightarrow\rightarrow(R_1-R_2)$
- $R_1∩R_2\rightarrow\rightarrow(R_2-R_1)$

***
#### Ejemplo
- Sea la relación $A = \{id, a_1,a_2,...,a_{m-1},a_m,a_{m+1},...,a_n\}$. 
- Sobre esta relación se define la siguiente [[Dependencia Multivaluada no Trivial]]$$id →→ a_ₘ / id, a_1,a_2,...,a_{m-1},a_{m+1},...,a_n$$
	- Esta dependencia viola la [[Cuarta Forma Normal según Dependencias Multivaluadas]] (4NF), ya que $id$ no es una [[Superclave]] de A si asumimos que la clave es ${id, a_ₘ}$ para determinar unívocamente una tupla.
- Solución (Descomposición sin pérdida en 4NF):
	- Para normalizar la relación, la descomponemos en dos relaciones, $A'$ y $R_{ₐₘ}$, de la siguiente manera:
    $$A'=\{id, a_1,a_2,...,a_{m-1},a_{m+1},...,a_n\}$$
	    - Esta relación contiene el determinante y todos los atributos que no participan en la DMV.
	    - Se cumple entonces que $$id\rightarrow a_1,a_2,...,a_{m-1},a_{m+1},...,a_n$$
	    - La segunda relación $$R_{a_m} = \{id, a_ₘ\}$$
		    - Esta relación contiene el determinante y el atributo multivaluado.
		    - Su clave primaria está compuesta por ambos atributos: $\{id, a_m\}$.
- Resultado:
	- Ambas relaciones, $A'$ y $R_{a_m}$, se encuentran ahora en $4NF$, eliminando la redundancia de datos.

***
#### Etiquetas
- #Anki 