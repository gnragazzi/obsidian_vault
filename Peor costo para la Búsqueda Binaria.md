Esta determinado por $$f(n)=1\ \ \ \ \ \text{ si }n=1$$$$f(n)=f(\lfloor{\frac{n}{2}}\rfloor)+1\ \ \ \ \ \text{ si } n>1$$
***
El término inferior proviene de que, el peor costo de encontrar un elemento es el costo de verificar si es el elemento del médio + el costo máximo de buscarlo en cualquiera de las 3 partes (mitad inferior, elemento intermedio, mitad superior). En símbolos$$f(n)=1+\max\{\text{costo de buscarlo en la mitad inferior}, 0, \text{costo de buscar en la mitad superior}\}$$Si el elemento del medio es $\lfloor{\frac{n+1}2}\rfloor$, entonces$$f(n)=1+max\{f(\lfloor{\frac{n+1}2}\rfloor-1),f(n-\lfloor{\frac{n+1}2}\rfloor\})$$
por las [[Propiedades Función Piso-Techo#^904eed|propiedades de las funciones piso/techo]] tenemos, entonces que$$f(n)=1+max\{f(\lceil{\frac{n}2}\rceil-1),f(\lfloor{\frac{n}2}\rfloor\})$$
En donde $\lceil{\frac{n}2}\rceil-1≤\lfloor{\frac{n}2}\rfloor$ que nos lleva al término inferior.
***
Siguiendo la [[Resolver Recurrencias|estrategia de resolver recurrencias]], llegamos a que el peor costo para encontrar un elemento $x$ entre $n$ elementos en una lista ordenada, utilizando búsqueda binaria es$$f(n)=\lfloor{\lg{n}}\rfloor+1$$