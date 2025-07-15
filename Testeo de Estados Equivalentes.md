Sean $p$ y $q$ estados de M, un AFD. Si $$∀w∈L(M): \hat{δ}(p,w) ∈F ⇔ \hat{δ}(q,w)^{[1]}\in F$$decimos que $p$ y $q$ son ***equivalentes***.
***
No es necesario que sean el mismo estado, solo que o o ambas den como resultado estados finales o ambas sean estados no finales.
Si dos estados no son equivalentes, decimos que son ***distinguibles***. Esto sucede si hay al menos una cadena w tal que uno de las $\hat\delta$ es final y el otro no.
[[Algoritmo de Tabla Completa]]  ^f07b74
***
[1]. [[Función de Transición Extendida - AFD]] 

#v2 