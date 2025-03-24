Tipo de [[Red Neuronal]] diseñada para trabajar con datos secuenciales.
Se diferencian de las RN tradicionales porque las salidas de neuronas en una capa puede ser usada como entrada a neuronas en la misma capa, lo que permite "recordar" información de entradas anteriores.
***
- Pueden procesar entradas de cualquier longitud 
- Para ello necesitan alguna forma de memoria 
- Así, la respuesta (salida) de una RNN depende, además de su entrada actual, de la información del pasado almacenada en su memoria
- Ejemplo RNN simple
- ![[Pasted image 20250324100745.png]]
***
![[Captura de pantalla 2025-03-17 a la(s) 12.18.09 p. m..png]]Su naturaleza Secuencial dificulta el paralelismo.
La solución son los [[Transformers]]
