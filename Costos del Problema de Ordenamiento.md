#### Definición
Sea:
- $N$=cantidad de elementos a ordenar
- $M$=tamaño de la memoria principal (en unidades de ítems de datos)
- $B$=Cantidad de elementos por página
- $n=N/B$ (cantidad de páginas para $N$ elementos)
entonces
- Si los datos entran en memoria principal: $O(N\;log\;N)$ accesos a MP (memoria principal).
- Si los datos no entran en memoria principal y dejamos a la memoria virtual el manejo de las páginas de disco: $\Omega(N\;log\;n)$ operaciones de $I/O$ 
- Si los datos no entran en memoria principal, y diseñamos un AMS $Θ(n\;log_{M/B}\; n)$ operaciones I/O
***
#### Etiquetas
- #Anki 