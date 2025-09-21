#### Definición
- Dada una tabla por segmentos, queremos determinar a partir de un número aleatorio $y=R$ cual es el valor de $x$ que le corresponde:
	- Por ejemplo, aquí el valor de $y$ será un valor en $(0,1)$ y $x$ un valor enre 0 y 2 (duración de reparación) 
	  ![[Pasted image 20250920220723.png|400]]
- Se genera una interpolación lineal según la Frecuencia Relativa Acumulada inferior y superior a $y$.
	- Por ej: si $y=0.83$, $F_I=0.66$ y $F_S=1.00$ y se tiene que $X_I=1.5\le x\le X_S=2.0$ 
- Luego, siguiendo propiedades de la trigonometría:
	- $$\frac{F_S-F_I}{X_S-X_I}=\frac{R-F_I}{X-X_I}$$
	- Despejando X, se tiene el valor esperado
	- En nuestro Ejemplo ![[Pasted image 20250920221344.png]]
***
#### Etiquetas
- #falta 