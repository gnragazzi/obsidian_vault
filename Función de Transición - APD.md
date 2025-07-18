$$δ:Q×(Σ∪{\lambda})×Γ→2^{Q×Γ^∗}$$
Es decir que la función de transición recibe una triupla. Está definida de la siguiente manera$$\delta(q,a,X)=\{(q,\gamma)|q∈Q\land\gamma\in \Gamma^* \}$$
- Es un conjunto de posibles estados (naturalmente es [[Determinismo - APD|no-deterministico]])
- $\gamma$ puede ser una palabra
- Si $\gamma=\lambda$ entonces se hace pop en la pila
- Si $\gamma=X$ la pila no se modifica
- Si $\gamma=YZ$, $X$ es reemplazado por $Z$ e $Y$ es puesto en la pila.
	- Creo que en este caso $Y\in\Gamma^*,Z\in\Gamma$  
***
#v2 