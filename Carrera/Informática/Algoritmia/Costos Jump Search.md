**Peor costo:**
Sean:
- $n$ el número de elementos de la lista
- $k$ el tamaño del salto (se saltan $k$ elementos)
- $m$ la cantidad de saltos que se necesitan para recorrer n, tal que$$m.k≤n<(m+1).k\text{ (1)}$$
Entonces se realizan, a lo sumo $m+k-1$ saltos para encontrar un elemento.
Por (1) sabemos que $m≤\frac{n}{k}<{m+1}$. Luego, por definición de [[Función Piso - Discretas|piso]], $m=\lfloor{\frac{n}{k}}\rfloor$. Por lo que el peor costo, es $$\lfloor{\frac{n}{k}}\rfloor+k-1$$
***
El costo se minimiza cuando $k=\lceil{\sqrt{n}}\rceil$ ¹
***
¹. [Compared to What?]
