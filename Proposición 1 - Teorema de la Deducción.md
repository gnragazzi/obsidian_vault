**Proposición 1** Si $\Gamma \vdash_{\mathcal{L}} (A \rightarrow B)$ entonces $\Gamma \cup \{A\} \vdash_{\mathcal{L}} B$, siendo $A$ y $B$ [[Sistema Formal L#^9688e4|fbfs]] de $\mathcal{L}$ y $\Gamma$ un conjunto (eventualmente vacío) de [[Sistema Formal L#^9688e4|fbfs]] de $\mathcal{L}$.
***
  **[[Deducción - Sistemas Formales|Demostración]]:** Lo que se debe hacer es dada una [[Deducción - Sistemas Formales|deducción]] de $(A \rightarrow B)$ a partir de $\Gamma$, construir una [[Deducción - Sistemas Formales|deducción]] de $B$ a partir de $\Gamma \cup {A}$.
$\vdots$                                            [[Deducción - Sistemas Formales|deducción]] de $(A \rightarrow B)$ a partir de $\Gamma$  
$k)$  $(A \rightarrow B)$  
$k+1)$ $A$                                                   hipótesis $(\in \Gamma \cup {A})$  
$k+2)$ $B$                                             [[Modus Ponens|MP]] entre $k)$ y $k+1)$
Luego se llegó a que $\Gamma \cup {A} \vdash_{\mathcal{L}} B$.  
c.q.d. █