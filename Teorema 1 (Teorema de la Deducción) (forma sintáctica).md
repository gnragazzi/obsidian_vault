Sean $A$ y $B$ [[Sistema Formal L#^9688e4|fbfs]] de $\mathcal{L}$ y sea $\Gamma$ un conjunto de [[Sistema Formal L#^9688e4|fbfs]] de $\mathcal{L}$ (que puede ser vacío),
$$\text{Si } \Gamma \cup \{A\} \vdash_{\mathcal{L}} B \text{ entonces } \Gamma \vdash_{\mathcal{L}} (A \rightarrow B)
$$
***
[[Proposición 1 - Teorema de la Deducción]] 
[[Corolario 1 - Teorema de la deducción]] 
***
**Demostración:**  
La demostración se hará por inducción sobre la cantidad de [[Sistema Formal L#^9688e4|fbfs]] que forman parte de la [[Deducción - Sistemas Formales|deducción]] de $B$ a partir de $\Gamma \cup {A}$. Para el paso base se supone que esta [[Deducción - Sistemas Formales|deducción]] tiene un solo miembro que es la misma $B$, entonces o $B$ es un [[Axioma|axioma]] de $\mathcal{L}$, o pertenece a $\Gamma \cup {A}$ (es decir $B \in \Gamma$ o $B \in {A}$). Teniendo esto en cuenta se debe hacer la [[Deducción - Sistemas Formales|deducción]] de $(A \rightarrow B)$ a partir de $\Gamma$.
- **Primer caso:** $B$ es un [[Axioma|axioma]] de $\mathcal{L}$,
    1. $B$  
            [[Axioma|Axioma]] de $\mathcal{L}$
    2. $(B \rightarrow (A \rightarrow B))$  
            [[Axioma|Axioma]] L1
    3. $(A \rightarrow B)$  
            [[Modus Ponens|MP]] entre 1) y 2)
    Luego $\Gamma \vdash_{\mathcal{L}} (A \rightarrow B)$
- **Segundo caso:** $B \in \Gamma$
       1. $B$  
            hipótesis
       2. $(B \rightarrow (A \rightarrow B))$  
            [[Axioma|Axioma]] L1
       3. $(A \rightarrow B)$  
            [[Modus Ponens|MP]] entre 1) y 2)
       Nuevamente $\Gamma \vdash_{\mathcal{L}} (A \rightarrow B)$
- **Tercer caso:** $B \in {A}$, en este caso $B = A$, por lo tanto hay que mostrar que
       $$\Gamma \vdash_{\mathcal{L}} (A \rightarrow A)$$
1. $(A \rightarrow ((A \rightarrow A) \rightarrow A))$
2. $((A \rightarrow ((A \rightarrow A) \rightarrow A)) \rightarrow ((A \rightarrow (A \rightarrow A)) \rightarrow (A \rightarrow A)))$
3. $((A \rightarrow (A \rightarrow A)) \rightarrow (A \rightarrow A))$
4. $(A \rightarrow (A \rightarrow A))$
5. $(A \rightarrow A)$

En esta última demostración no hizo falta utilizar ninguna [[Sistema Formal L#^9688e4|fbf]] de $\Gamma$ porque $(A \rightarrow A)$ es un [[Teorema (Lógica) - Definición|teorema]] de $\mathcal{L}$, pero es claro que $\Gamma \vdash_{\mathcal{L}} (A \rightarrow A)$. Por lo tanto aquí también se mostró que $\Gamma \vdash_{\mathcal{L}} (A \rightarrow B)$, con lo que se completa la demostración del paso base.
***
Supongamos ahora que la [[Deducción - Sistemas Formales|deducción]] de $B$ a partir de $\Gamma \cup {A}$ es una sucesión de $n$ miembros, siendo $n \geq 1$, y que la proposición se verifica para todas las [[Sistema Formal L#^9688e4|fbfs]] $C$ que pueden deducirse a partir de $\Gamma \cup {A}$ por medio una sucesión de _menos de_ $n$ pasos. Esta será nuestra hipótesis inductiva. Ahora hay que considerar cuatro casos diferentes:
- **Primer caso:** $B$ es un [[Axioma|axioma]] de $\mathcal{L}$. Este caso es exactamente igual al primer caso del paso base, es decir que se debe demostrar que $\Gamma \vdash_{\mathcal{L}} (A \rightarrow B)$, y esto se hace de la misma forma en que se hizo antes.
- **Segundo caso:** $B \in \Gamma$. Nuevamente se demuestra $\Gamma \vdash_{\mathcal{L}} (A \rightarrow B)$ de la misma que en el caso base.
- **Tercer caso:** $B \in {A}$, es decir que $B$ es $A$, y la demostración de $\Gamma \vdash_{\mathcal{L}} (A \rightarrow A)$ es la misma mostrada antes.
- **Cuarto caso:** $B$ se obtiene de dos [[Sistema Formal L#^9688e4|fbfs]] anteriores de la demostración mediante una aplicación de [[Modus Ponens|MP]]. Estas dos [[Sistema Formal L#^9688e4|fbfs]] necesariamente tendrán las formas $C$ y $(C \rightarrow B)$ y cada una de ellas puede ciertamente deducirse de $\Gamma \cup {A}$ mediante una sucesión de _menos de_ $n$ pasos. En cada caso, basta con omitir los miembros siguientes de la [[Deducción - Sistemas Formales|deducción]] original, y lo que queda es la sucesión deseada. (ver Observación 1-b)). Entonces, de lo anterior tenemos que $\Gamma \cup {A} \vdash_{\mathcal{L}} C$ y $\Gamma \cup {A} \vdash_{\mathcal{L}} (C \rightarrow B)$, y aplicando la hipótesis de inducción se llega a que $\Gamma \vdash_{\mathcal{L}} (A \rightarrow C)$ y $\Gamma \vdash_{\mathcal{L}} (A \rightarrow (C \rightarrow B))$.

Entonces, ahora se puede realizar la [[Deducción - Sistemas Formales|deducción]] requerida, $\Gamma \vdash_{\mathcal{L}} (A \rightarrow B)$, como sigue:
$\vdots$  
$k)$ $(A \rightarrow C)$          [[Deducción - Sistemas Formales|deducción]] de $(A \rightarrow C)$ a partir de $\Gamma$  
$k+1)$  
$\vdots$  
$l)$ $(A \rightarrow (C \rightarrow B))$  [[Deducción - Sistemas Formales|deducción]] de $(A \rightarrow (C \rightarrow B))$ a partir de $\Gamma$  
$l+1)$ $(A \rightarrow (C \rightarrow B)) \rightarrow ((A \rightarrow C) \rightarrow (A \rightarrow B))$   [[Axioma|Axioma]] L2  
$l+2)$ $((A \rightarrow C) \rightarrow (A \rightarrow B))$       [[Modus Ponens|MP]] entre $l)$ y $l+1)$  
$l+3)$ $(A \rightarrow B)$          [[Modus Ponens|MP]] entre $k)$ y $l+2)$

De este modo se demostró que $\Gamma \vdash_{\mathcal{L}} (A \rightarrow B)$ en los cuatro casos. Así pues, por el principio de inducción matemática, la proposición se verifica cualquiera que sea el número de [[Sistema Formal L#^9688e4|fbfs]] de la [[Deducción - Sistemas Formales|deducción]] de $B$ a partir de $\Gamma \cup {A}$.  
c.q.d. █