Una [[Fórmula - LPO|fórmula]] $\varphi$ de un [[Alfabeto - LPO|lenguaje de primer orden]] $L_\sigma$ es **consecuencia** de un conjunto de fórmulas de $L_\sigma$, $\Phi$, y se denota $\varphi \in \operatorname{Cons}(\Phi)$, si y sólo si para toda [[Interpretación - LPO|interpretación]] $\mathcal{I}$ tal que $\mathcal{I} \models \Phi$ se cumple que $\mathcal{I} \models \varphi$, es decir:
$$\mathcal{I} \models \Phi \cup \{\varphi\}$$
o dicho de otra manera:
$$\varphi \in \operatorname{Cons}(\Phi) \quad \text{si y sólo si} \quad \Phi \cup \{\neg \varphi\} \text{ es insatisfacible}.$$