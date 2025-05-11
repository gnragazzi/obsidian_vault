Denotaremos con:
- $U(S)$ la [[Utilidad - IA|utilidad]] del estado $s$ para el [[Agentes Basados en Utilidad|agente]] que está tomando las decisiones.
- $a$: Una acción no deterministica
- $Resultado_i(a)$: Conjunto de posibles estados resultantes de aplicar $a$, donde el índice $i$ varía en el rango de los posibles resultados.
- $E$: evidencia disponible al agente sobre el mundo
- $Realizar(a)$: proposición de que la acción $a$ es ejecutada en el estado actual.
- $P(Resultado_i(a)|Realizar(a),E)$: probabilidad asignada por el agente a cada resultado posible.
Podemos calcular la *Utilidad Experada* de una acción dada la evidencia $UE(a|E)$, usando la fórmula: $$UE(a|E)=\sum_iP(Resultado_i(a)|E,Realizar(a)).U(Resultado_i(a))$$
***
El principio de la Utilidad Esperada Máxima establece que un agente racional siempre debería elegir aquella acción que maximiza la utilidad esperada del agente.

