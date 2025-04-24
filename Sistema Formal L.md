[[Sistema Formal - Definición]] 
***
**Definición 1** _El sistema formal $\mathcal{L}$ del [[Lógica Proposicional|cálculo proposicional]] se define como:_
- **Alfabeto** de símbolos (infinito): $\rightarrow$, $\neg$, $($, $)$, $p_1, p_2, p_3, \dots$
- **Conjunto de fbfs**, especificado a través de una regla inductiva ([[Gramática|gramática]]) con tres partes:  
    (i) $p_i$ es una fbf para todo $i \geq 1$.  
    (ii) Si $A$ y $B$ son fbfs, entonces $(\neg A)$ y $(A \rightarrow B)$ son fbfs.  
    (iii) El conjunto de todas las fbfs es el generado por (i) e (ii). ^9688e4
- **Axiomas.** Hay infinitos [[Axioma|axiomas]], entonces en lugar de mencionarlos a todos, se los va a especificar por medio de tres _esquemas de axiomas._  
    Sean las fbfs $A$, $B$ y $C$; las fórmulas bien formadas obtenidas por los siguientes esquemas son axiomas de $\mathcal{L}$:
    **L1** : $(A \rightarrow (B \rightarrow A))$  
    **L2** : $((A \rightarrow (B \rightarrow C)) \rightarrow ((A \rightarrow B) \rightarrow (A \rightarrow C)))$  
    **L3** : $(((\neg A) \rightarrow (\neg B)) \rightarrow (B \rightarrow A))$
- **Reglas de inferencia.** El sistema $\mathcal{L}$ tiene una única regla de inferencia, el _[[Modus Ponens]]_ 
***
[[Propiedades de un Sistema Formal]] 