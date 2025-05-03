ES UNA NOTACIÓN ESPECIAL PARA DESCRIBIR EL ESTADO ACTUAL DEL AUTÓMATA (UNA DESCRIPCIÓN INSTANTÁNEA). UNA CONFIGURACIÓN DE UN APD ES UNA TRIUPLA $(q, w, \gamma) \in Q \times \Sigma^* \times \Gamma^*$ DONDE:
- $q$ es el estado actual,
- $w$ es la cadena remanente en la entrada (aún no analizada),
- $\gamma$ es el contenido de la pila,
LUEGO, UN MOVIMIENTO DE UN APD SE REPRESENTA RELACIONANDO DOS CONFIGURACIONES DE LA SIGUIENTE MANERA:
$$(q, aw, Z\alpha) \vdash (p, w, \gamma\alpha) \text{ si } \delta(q, a, Z) \text{ contiene a } (p, \gamma)$$
***
$\mathrel{\vdash\!\!\!^i}$ movimiento en i pasos
$\mathrel{\vdash\!\!\!^+}$ clausura transitiva
$\mathrel{\vdash\!\!\!^*}$ clausura reflexo-transitiva
***
- **Configuración Inicial**: $(q_0, w, Z_0)$ con $w \in \Sigma^*$.
- **Configuración Final**: $(q, \lambda, \alpha)$, con $q \in F$ y $\alpha \in \Gamma^*$, o  $(q, \lambda, \lambda)$, con $q \in Q$.
Una cadena $w \in \Sigma^*$ es aceptada por un APD si partiendo de una configuración inicial llega a una configuración final.