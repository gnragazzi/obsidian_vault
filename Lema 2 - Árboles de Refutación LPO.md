Para todo [[Fórmula Satisfacible - LPO|conjunto satisfacible]] de [[Fórmula - LPO|fórmulas]] $\Phi$ se tiene que:
1. Si $(\forall x, \varphi) \in \Phi$, entonces $\Phi \cup { \varphi(x/t) }$ es satisfacible, para todo [[Término - Lógica Primer Orden|término]] $t$ adecuado para [[Sustitución de variables en Fórmulas|sustituir]] a $x$ en $\varphi$.
2. Si $(\exists x, \varphi) \in \Phi$, entonces $\Phi \cup { \varphi(x/c) }$ es satisfacible, para todo símbolo de constante $c$ que no figure en ninguna de las fórmulas del conjunto $\Phi$.
3. Si $\neg(\forall x, \varphi) \in \Phi$, entonces $\Phi \cup { \neg \varphi(x/c) }$ es satisfacible, para todo símbolo de constante $c$ que no figure en ninguna de las fórmulas del conjunto $\Phi$.
4. Si $\neg(\exists x, \varphi) \in \Phi$, entonces $\Phi \cup { \neg \varphi(x/t) }$ es satisfacible, para todo término $t$ adecuado para sustituir a $x$ en $\varphi$.
***
![[Pasted image 20250513075218.png]]
***
Demostración
***
[[Reglas adicionales - Árboles de Refutación - LPO]] 