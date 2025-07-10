### Definición
Una configuración representa el estado actual en el que se encuentra un [[Autómata Finito Determinístico|AFD]] y la porción de [[Cadena - Lenguajes|cadena]] de entrada que aún no se ha consumido. Por lo tanto es un par $(q,x)$ 
### Definición de la relación
Se puede definir una relación que nos permite obtener una configuración a partir de otra, de la siguiente manera$$(q,ax)⊢(q',x) \text{ donde } a∈Σ, ⇔ δ(q,a)=q'$$
### Clausura Reflexo-Transitiva de $⊢$ y definición de 
> También se puede definir esta relación para indicar como obtener una configuración, a partir de otra, en 0 o más pasos $(⊢^*)$ como la [[Clausura Reflexo Transitiva|clausura reflexo transitiva]] de $⊢$. 
> Entonces, es posible dar la siguiente definición de lenguaje aceptado por un $M = (Q, Σ, δ, q_0 , F )$ como:$$L(M)=\{x∈Σ^*/∃f∈F,(q_0,x)⊢^*(f,λ)\}$$
### Etiquetas
> #v2