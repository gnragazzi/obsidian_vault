De archivos:
```
f = open(<nombre>,<método>,encoding="utf-8")
```
- recordar que hay que cerrar con `f.close()`
- se puede hacer en un try - finally block
- hay una sintaxis [[with]] que debería aprender y se usa para utilizar archivos.
- Los métodos son cadenas, que pueden terminar con b. En tal caso, son binarios y se utilizan con objetos byte
- Para leer información del archivo abierto se usa el método .read()
	- Esta función vacía el buffer de entrada
	- Método .seek(0) devuelve el puntero del archivo al comienzo
	- método .tell() puede decir en dónde se encuentra el puntero
- Para escribir información en el archivo abierto se usa el método write()
---
De la pantalla:
```a = input(<mensaje:string>)```
- Tendrá el valor ingresado por pantalla
---
De archivos XML
```
import xml.etree.ElementTree as ET
tree = ET.parse(archivo_entrada)
root = tree.getroot()
```
- A partir de ahora, root es el nodo raiz del archivo xml cuya dirección está determinada por `archivo_entrada`.
- tree es un objeto de la clase ElementTree (que se utiliza para manipular el archivo como un todo)
- root es un objeto de la clase Element, que se utiliza para manipular nodos.
- `<Element>.tag` => el nombre del tag
- `<Element>.attrib` => [[dictionary|diccionario]] con nombre_atributo: valor
- `<Element>` es iterable, pero muestra únicamente a sus hijos. Para iterar sobre si mismo y sus hijos, hay que crear un iterable con `<Element>.iter(tag=None)`
---
De linea de comandos
```
import sys
n = len(sys.argv) #tamaño de lista de argumentos (el índice 0 tiene el nombre del archivo)

for arg in sys.argv: ... # cada argumento en la lista de argumentos
```