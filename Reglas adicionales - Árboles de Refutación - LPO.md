El [[Lema 2 - Árboles de Refutación LPO|lema precedente]] sugiere considerar los siguientes esquemas:
$$\begin{array}{ll} \mathbf{R}_{\forall} & \dfrac{(\forall x\, \varphi)}{\varphi(x/t)} \quad \text{donde } t \text{ es cualquier término sin variables.} \\ \\ \mathbf{R}_{\exists} & \dfrac{(\exists x\, \varphi)}{\varphi(x/c)} \quad \text{donde } c \text{ es una constante, con restricciones.} \\ \\ \mathbf{R}_{\neg \forall} & \dfrac{\neg(\forall x\, \varphi)}{\neg \varphi(x/c)} \quad \text{donde } c \text{ es una constante, con restricciones.} \\ \\ \mathbf{R}_{\neg \exists} & \dfrac{\neg(\exists x\, \varphi)}{\neg \varphi(x/t)} \quad \text{donde } t \text{ es cualquier término sin variables.} \end{array}$$
El agregado “con restricciones” que figura en las reglas $\mathbf{R}_{\exists}$ y $\mathbf{R}_{\neg \forall}$ recuerda que el símbolo de constante $c$ no puede ser elegido arbitrariamente.
Notemos que todo término en el que no figuran variables o es una constante o se obtiene de combinar símbolos de función con constantes, y es adecuado para sustituir las apariciones libres de cualquier variable en cualquier fórmula.
Dada una [[Fórmula - LPO|fórmula]] $\varphi$ definimos $\varphi(x/t)$ de la siguiente manera:
- Si $x$ [[Variables Libres - Apariciones Libres y Ligadas de Variables - LPO|no ocurre libre]] en $\varphi$: $\varphi(x/t)$ es $\varphi$.
- Si $x$ ocurre libre en $\varphi$: $\varphi(x/t)$ es la fórmula obtenida al reemplazar todas las ocurrencias libres de $x$ por $t$.
***
![[Pasted image 20250513075209.png]]
***
![[Pasted image 20250513083344.png]]