Sea $P$ una [[Fórmula Lógica|fórmula]] y supongamos $Var(P)⊆\{x_1,x_2,...,x_n\}$. Por el [[Corolario 1 de la Extensión de la Función de Valuación]] para cada n-upla $\overline{a}=(a_1,a_2,...,a_n)∈B^n$ hay una valuación $v_{\overline{a}}$ tal que $$v_{\overline{a}}(x_i)=a_i$$ para $1≤i≤n$. 
De acuerdo al [[Teorema 2 - Procedimiento para Evaluar una Fórmula]] $v_{\overline{a}}(P)$ se calcula sustituyendo cada $x_i$ por sus valores correspondientes $a_i$ y evaluando según los conectivos.
Si listamos todas las n-uplas $\overline{a}∈B^n$ y a la derecha escribimos el valor de verdad $v_{\overline{a}}(P)$, obtenemos una tabla o matriz de $2^n$ filas y $n+1$ columnas formadas por elementos de $B$. A esta tabla la denominamos ***Tabla de Verdad de la fórmula P***.
***
[[Función Booleana de n Variables]] 
***
![[Pasted image 20250331093727.png]]
***
Observemos que si en la columna $n+1$ obtenemos unicamente $⊤$, entonces $P$ es una [[Tautología, Contradicción y Contingencia#^6807de|tautología]], obtenemos unicamente ⊥, es una contradicción; caso contrario es una contingencia.