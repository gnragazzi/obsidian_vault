Es una notación especial para describir el estado actual del autómata (una descripción instantánea). 
Una configuración de un apd es una triupla $(q, w, \gamma) \in Q \times \Sigma^* \times \Gamma^*$ donde:
- $q$ es el estado actual,
- $w$ es la cadena remanente en la entrada (aún no analizada),
- $\gamma$ es el contenido de la pila,
Luego, un movimiento de un APD se representa relacionando dos configuraciones de la siguiente manera:
$$(q, aw, Z\alpha) \vdash (p, w, \gamma\alpha) \text{ si } \delta(q, a, Z) \text{ contiene a } (p, \gamma)$$
***
$\mathrel{\vdash\!\!\!^i}$ movimiento en i pasos
$\mathrel{\vdash\!\!\!^+}$ clausura transitiva
$\mathrel{\vdash\!\!\!^*}$ clausura reflexo-transitiva
***
- **Configuración Inicial**: $(q_0, w, Z_0)$ con $w \in \Sigma^*$.
- **Configuración Final**: $(q, \lambda, \alpha)$, con $q \in F$ y $\alpha \in \Gamma^*$, o  $(q, \lambda, \lambda)$, con $q \in Q$.
Una cadena $w \in \Sigma^*$ es aceptada por un APD si partiendo de una configuración inicial llega a una configuración final.