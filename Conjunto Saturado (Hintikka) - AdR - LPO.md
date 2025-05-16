Un conjunto $\mathbb{H} \subseteq \mathbb{F}$ se dice _saturado_, o un _conjunto de Hintikka_, si satisface las siguientes condiciones:
**H.1** Una [[Fórmula - LPO|fórmula]] y su negación no pueden estar ambas en $\mathbb{H}$.
**H.2** Si $\lnot \lnot \varphi \in \mathbb{H}$, entonces $\varphi \in \mathbb{H}$.
**H.3** Si $(\varphi \lor \psi) \in \mathbb{H}$, entonces $\varphi \in \mathbb{H}$ o $\psi \in \mathbb{H}$.
**H.4** Si $\lnot (\varphi \lor \psi) \in \mathbb{H}$, entonces $\lnot \varphi \in \mathbb{H}$ y $\lnot \psi \in \mathbb{H}$.
**H.5** Si $(\varphi \land \psi) \in \mathbb{H}$, entonces $\varphi \in \mathbb{H}$ y $\psi \in \mathbb{H}$.
**H.6** Si $\lnot (\varphi \land \psi) \in \mathbb{H}$, entonces $\lnot \varphi \in \mathbb{H}$ o $\lnot \psi \in \mathbb{H}$.
**H.7** Si $(\varphi \rightarrow \psi) \in \mathbb{H}$, entonces $\lnot \varphi \in \mathbb{H}$ o $\psi \in \mathbb{H}$.
**H.8** Si $\lnot (\varphi \rightarrow \psi) \in \mathbb{H}$, entonces $\varphi \in \mathbb{H}$ y $\lnot \psi \in \mathbb{H}$.
**H.9** Si $(\forall x, \varphi) \in \mathbb{H}$, entonces $\varphi(x/t) \in \mathbb{H}$ para todo término $t$ sin variables.
**H.10** Si $\lnot (\forall x, \varphi) \in \mathbb{H}$, entonces $\lnot \varphi(x/c) \in \mathbb{H}$ para algún símbolo de constante $c$.
**H.11** Si $(\exists x, \varphi) \in \mathbb{H}$, entonces $\varphi(x/c) \in \mathbb{H}$ para algún símbolo de constante $c$.
**H.12** Si $\lnot (\exists x, \varphi) \in \mathbb{H}$, entonces $\lnot \varphi(x/t) \in \mathbb{H}$ para todo término $t$ sin variables.