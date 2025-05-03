Un APD se define como una **7-tupla**:
$M=(Q,Σ,Γ,δ,q_0,Z_0,F)$
donde:

1. $Q$: Conjunto finito de _estados_.
2. $Σ$: Alfabeto de entrada (finito).
3. $Γ$ Alfabeto de la _pila_ (símbolos que pueden almacenarse).
4. $δ$: [[Función de Transición de Autómatas Push-Down|Función de transición]]:  $$δ:Q×(Σ∪{\lambda})×Γ→2^{Q×Γ^∗}$$
5. $q_0∈Q$ Estado inicial.
6. $Z_0∈Γ$: Símbolo inicial de la pila.
7. $F⊆Q$: Conjunto de estados finales (de aceptación).
***
Características
- [[Movimientos de un APD]] 
- [[Aceptación de una cadena por un APD]] 
- [[Configuraciones de un APD]] 
- 