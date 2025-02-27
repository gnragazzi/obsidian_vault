- $\min_{x∈ℝ}\lfloor{f(x)}\rfloor≤\min_{x∈ℝ}f(x)$ 
- $\min_{x∈ℝ}\lceil{f(x)}\rceil=\lceil{\min_{x∈ℝ}f(x)}\rceil$ 
***
Propiedades que Relacionan Piso y Techo ^904eed
- $\lfloor{\frac{x}2}\rfloor≤\lceil{\frac{x}2}\rceil≤\lfloor{\frac{x+1}2}\rfloor$
- $\lceil{\frac{x}2}\rceil=\lfloor{\frac{x+1}2}\rfloor$ 
- $\lfloor{\frac{x}2}\rfloor+\lceil{\frac{x}2}\rceil=x$
- $\lfloor{\lfloor{\frac{n}{l}}\rfloor/m}\rfloor=\lfloor{\frac{n}{lm}}\rfloor$  (por ejemplo $\lfloor{\lfloor{\frac{n}{2}}\rfloor/2}\rfloor=\lfloor{\frac{n}{4}}\rfloor$  con $l=m=2$)¹
***
¹.$$k=\lfloor{\frac{n}{lm}}\rfloor⇒k≤\frac{n}{lm}<k+1\text{ por definición de función piso}$$$$⇒mk≤\frac{n}{l}<mk+m$$$$⇒mk≤\lfloor{\frac{n}{l}}\rfloor<mk+m$$
$$⇒k≤\lfloor{\frac{n}{l}}\rfloor/m<k+1⇒\lfloor{\lfloor{\frac{n}{l}}\rfloor/m}\rfloor=k=\lfloor{\frac{n}{lm}}\rfloor$$