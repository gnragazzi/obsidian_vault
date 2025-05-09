Sea $\varphi$ una fórmula de $L_\sigma(\mathcal{I})$ de [[Grado de Complejidad de una fórmula - LPO|complejidad]] $0$, entonces por la definición de complejidad es una [[Fórmulas Atómicas - LPO|fórmula atómica]]. Por lo tanto hay un único $k \geq 1$, un único $P \in \mathcal{P}$ de aridad $k$ y una única $k$-upla de [[Término - Lógica Primer Orden|términos]] $t_1, \dots, t_k$ tales que $\varphi = P(t_1, \dots, t_k)$. Como se dijo anteriormente, los $t_i$ deben ser términos del lenguaje $L_\sigma(\mathcal{I})$ y por lo tanto designan elementos $\mathcal{I}'(t_i)$([[Interpretación - LPO|ref]]) del universo $U$, para $i = 1, \dots, k$. Luego la $k$-upla $(\mathcal{I}'(t_1), \mathcal{I}'(t_2), \dots, \mathcal{I}'(t_k)) \in U^k$.
Entonces definimos:$$V_{\mathcal{I}}(\varphi) = \top \quad \text{si } (\mathcal{I}'(t_1), \mathcal{I}'(t_2), \dots, \mathcal{I}'(t_k)) \in P^{\mathcal{I}}$$$$V_{\mathcal{I}}(\varphi) = \bot \quad \text{si } (\mathcal{I}'(t_1), \mathcal{I}'(t_2), \dots, \mathcal{I}'(t_k)) \notin P^{\mathcal{I}}$$Sea $comp(\varphi) = n > 0$ y supongamos que hemos definido $V_{\mathcal{I}}(\psi)$ para toda fórmula $\psi$ de $L_\sigma(\mathcal{I})$ tal que $comp(\psi) < n$. Si $\varphi$ es una fórmula de complejidad $n$, se podía presentar uno, y sólo uno, de los siguientes casos:
1. Existe una única fórmula $\psi$ de $L_\sigma(\mathcal{I})$ tal que $\varphi = \neg \psi$.
2. Existe un único par de fórmulas $\psi, \eta$ de $L_\sigma(\mathcal{I})$ tal que $\varphi = (\psi \vee \eta)$.
3. Existe un único par de fórmulas $\psi, \eta$ de $L_\sigma(\mathcal{I})$ tal que $\varphi = (\psi \wedge \eta)$.
4. Existe un único par de fórmulas $\psi, \eta$ de $L_\sigma(\mathcal{I})$ tal que $\varphi = (\psi \rightarrow \eta)$.
5. Existe una única fórmula $\psi$ de $L_\sigma(\mathcal{I})$ y una única variable $x$ tal que $\varphi = (\forall x \ \psi)$.
6. Existe una única fórmula $\psi$ de $L_\sigma(\mathcal{I})$ y una única variable $x$ tal que $\varphi = (\exists x \ \psi)$.
Como en los casos $1, 2, 3$ y $4$ se tiene que $comp(ψ) < n$ y $comp(η) < n$, por la hipótesis inductiva  están definidos los valores de verdad $V_{\mathcal{I}}(ψ)$ y $V_{\mathcal{I}} (η)$. Entonces $V_{\mathcal{I}}(φ)$ es:
- En el caso 1, $V_{\mathcal{I}}(\varphi) \overset{def}{=} \neg V_{\mathcal{I}}(\psi)$.
- En el caso 2, $V_{\mathcal{I}}(\varphi) \overset{def}{=} V_{\mathcal{I}}(\psi) \vee V_{\mathcal{I}}(\eta)$.
- En el caso 3, $V_{\mathcal{I}}(\varphi) \overset{def}{=} V_{\mathcal{I}}(\psi) \wedge V_{\mathcal{I}}(\eta)$.
- En el caso 4, $V_{\mathcal{I}}(\varphi) \overset{def}{=} V_{\mathcal{I}}(\psi) \rightarrow V_{\mathcal{I}}(\eta)$.

O también lo podemos definir $V_{\mathcal{I}}(\varphi)$ como:
- En el caso 1, $V_{\mathcal{I}}(\varphi) \overset{def}{=} \top$ si y sólo si $V_{\mathcal{I}}(\psi) = \bot$.
- En el caso 2, $V_{\mathcal{I}}(\varphi) \overset{def}{=} \top$ si y sólo si $V_{\mathcal{I}}(\psi) = \top$ o $V_{\mathcal{I}}(\eta) = \top$.
- En el caso 3, $V_{\mathcal{I}}(\varphi) \overset{def}{=} \top$ si y sólo si $V_{\mathcal{I}}(\psi) = \top$ y $V_{\mathcal{I}}(\eta) = \top$.
- En el caso 4, $V_{\mathcal{I}}(\varphi) \overset{def}{=} \top$ si y sólo si $V_{\mathcal{I}}(\psi) = \bot$ o $V_{\mathcal{I}}(\eta) = \top$.

Para considerar los casos 5 y 6, observemos primero que $\varphi$ es una fórmula que puede tener [[Variables Libres - Apariciones Libres y Ligadas de Variables - LPO|variables libres]], pero en particular $x$ está ligada en ella. Sin embargo $\psi$ tiene a $x$ entre sus variables libres, por lo tanto, para cualquier elemento $a \in U$ se tiene que $\psi(x/a)$ es una fórmula de $L_\sigma(\mathcal{I})$ y dado que $comp(\psi(x/a)) = comp(\psi) < n$, por hipótesis inductiva resulta que $V_{\mathcal{I}}(\psi(x/a))$ está definido para todo $a \in U$.
En el caso 5 definimos$$V_{\mathcal{I}}(\varphi) \overset{def}{=} \top \quad \text{si y sólo si } V_{\mathcal{I}}(\psi(x/a)) = \top \quad \text{para todo elemento } a \in U.$$En el caso 6 definimos$$V_{\mathcal{I}}(\varphi) \overset{def}{=} \top \quad \text{si y sólo si existe \textit{al menos un} elemento } a \in U \text{ tal que } V_{\mathcal{I}}(\psi(x/a)) = \top.$$ ^80db7d