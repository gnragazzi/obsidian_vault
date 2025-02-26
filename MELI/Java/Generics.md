Es la utilización de *placeholder_types*, es decir que son ***tipos parametrizados***.
Permiten crear clases, interfaces, métodos que actúan en los que los tipos de datos sobre los que actúan son transmitidos como parámetros.
***
Características
- Desde jdk 5
- No soportan tipos primitivos (hay que usar Integer en lugar de int, etc...)
- Se emplea el "operador diamante", < > para especificar un genérico.
- Se declaran con letras mayúsculas (convención)
- Se puede delimitar los tipos a usar `<T extends Number>` (solo se podrán usar clases que sean sub-clases de Number).
- ![[Captura de pantalla 2025-02-26 a la(s) 3.42.48 p. m..png]]