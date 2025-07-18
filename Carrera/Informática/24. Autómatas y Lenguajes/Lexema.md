### Definición

Secuencia de [[Símbolo|caracteres]] en el programa fuente que a partir de un [[Patrón - Análisis Lexicográfico|patrón]], unifica con un [[Token]].

***
### Ejemplo

Si tenemos la declaración `int edad = 25;`, podemos identificar:
- `int`: Es un **lexema** que coincide con el **patrón** de "palabras clave" y se le asigna el **token** `palabra_clave_int`.
    
- `edad`: Es un **lexema** que coincide con el **patrón** de "identificador" (ej: `[a-zA-Z][a-zA-Z0-9]*`) y se le asigna el **token** `identificador`.
    
- `25`: Es un **lexema** que coincide con el **patrón** de "número" y se le asigna el **token** `numero_entero`.
***
#v2 