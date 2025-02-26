un Stream es una secuencia de elementos que puede ser procesada en paralelo o en serie.

***
- Permiten crear flujos de datos continuos para procesar con operadores
- Permite
	- filter
	- map
	- sorted
	- foreach
	- reduce
- Son inmutables
- Se pueden crear desde colecciones
	- set, list, map, etc...
- A partir de java 8.
- Permite procesar colecciones de datos.
***
Ejemplos
```
public static void primtStream(){
	List<String> names = getStringArray();
	names.stream().forEach(System.out::println);
}
```
Notar que
- .stream() devuelve un stream con los elementos de la colección. 
- .forEach() se aplica con cada elemento del stream
- Como argumento de la función intermedia se puede usar [[Expresión Lambda|expresiones lambda]] o [[Referencias a Métodos]].
![[Captura de pantalla 2025-02-26 a la(s) 4.58.49 p. m..png]]

![[Captura de pantalla 2025-02-26 a la(s) 4.59.10 p. m..png]]

![[Captura de pantalla 2025-02-26 a la(s) 4.59.19 p. m..png]]

![[Captura de pantalla 2025-02-26 a la(s) 4.59.28 p. m..png]]

![[Captura de pantalla 2025-02-26 a la(s) 4.59.41 p. m..png]]