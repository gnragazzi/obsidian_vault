Una **demostración** en $\mathcal{L}$ es [[Sucesión|sucesión]] finita de [[Sistema Formal L#^9688e4|fórmulas bien formadas]] $A_1, A_2, \dots, A_n$, tal que para todo $i$, con $1 \leq i \leq n$,
- (a) $A_i$ es un axioma de $\mathcal{L}$,
- (b) o bien se deduce de miembros anteriores de la sucesión digamos $A_j$ y $A_k$, con $j < i, k < i$, como consecuencia directa de la aplicación de la regla de inferencia **[[Modus Ponens|MP]]**.
***
Una demostración obtenida de esta manera será una demostración de $A_n$ en $\mathcal{L}$, y también se dirá que $A_n$ es un **[[Teorema (Lógica) - Definición |teorema]]** de $\mathcal{L}$.
***
**Observación 1**
1. Es claro que en la definición anterior, $A_j$ y $A_k$ necesariamente deben ser de las formas $B$ y $(B \rightarrow A_i)$ respectivamente, o viceversa.
2. Si $A_1, A_2, \dots, A_n$ es una demostración en $\mathcal{L}$ y $k < n$, entonces  
      $A_1, A_2, \dots, A_k$ es también una demostración en $\mathcal{L}$.  
      Evidentemente, satisface la definición, de modo que es un teorema de $\mathcal{L}$.
3. Los axiomas de $\mathcal{L}$ son ciertamente teoremas de $\mathcal{L}$. Sus demostraciones en $\mathcal{L}$ son sucesiones con un solo miembro.
