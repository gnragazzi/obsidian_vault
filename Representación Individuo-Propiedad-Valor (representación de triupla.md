```
prop(Individuo, Propiedad, Valor)
```
Por ejemplo, para decir que el lapiz 7 tiene color rojo, diría
```
prop(lapiz7, color , rojo)
```
***
Usos no tan inmediatos:
- Para representar que un objeto es algo, se pueden usar 2 alternativas:
	1. `prop(objeto, type, algo)` donde `type` es una palabra reservada para describir que un objeto es de de cierto tipo
	2. `prop(objeto,algo,verdadero)` para representar que es cierto que objeto es algo.
- *Cosificación (reification)*
	- Significa convertir algo en individuo.
	- Por ejemplo, si tenemos que la reserva “la comisión 2 del curso cs422 está programada a las 10:30 en el aula cc208.” se puede *cosificar* la reserva (en el siguiente ejemplo, se le da el nombre r123) y representarla como
		- `prop(r123, curso, cs422). `
		- `prop(r123, seccion, 2). `
		- `prop(r123, hora, 1030). `
		- `prop(r123, aula, cc208).`
	- Agregar propiedades (por ejemplo, quién da la clase o cuanto dura) es inmediato, lo que hace flexible a la representación 
- 
***
Esta representación tiene su forma visual en los [[Grafos de Conocimiento]] 