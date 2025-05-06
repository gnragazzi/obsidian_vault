Podemos determinar las [[Apariciones Libres y Ligadas de Variables|variables libres]] de una [[Fórmulas de la Lógica de Primer Orden|fórmula]] $\varphi$ calculando la función $Libres(\varphi)$, la que se define recursivamente de la siguiente manera:
- Si $\varphi$ es una [[Fórmulas Atómicas - LPO|fórmula atómica]], entonces $Libres(\varphi)$ es el conjunto de [[Alfabeto de la Lógica de Primer Orden|variables]] que ocurren en $\varphi$.
- En cualquier otro caso:
    - Si $\varphi$ es $\neg \psi$ entonces $Libres(\varphi) \overset{\text{def}}{=} Libres(\psi)$.
    - Si $\varphi$ es $(\psi \lor \eta)$, o $(\psi \land \eta)$ o $(\psi \rightarrow \eta)$ entonces $Libres(\varphi) \overset{\text{def}}{=} Libres(\psi) \cup Libres(\eta)$
    - Si $\varphi$ es $(\forall x \ \psi)$ o $(\exists x \ \psi)$ entonces $Libres(\varphi) \overset{\text{def}}{=} Libres(\psi) - \{x\}$.
Una variable $x$ se dice _ligada_ en $\varphi$ si $\varphi = (\forall x \ \psi)$ o $\varphi = (\exists x \ \psi)$.
