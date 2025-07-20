###### Demostración

Sean $L_1$ y $L_2$ dos LLC. Si los LLC son cerrados bajo la operación de complemento, entonces $$L=\overline{\overline{L_1}\cup\overline{L_2}}$$es un LLC.
Pero, utilizando las leyes de DeMorgan, podemos ver que $$\overline{\overline{L_1}\cup\overline{L_2}}=L_1∩L_2$$
Como se vio, [[Demostración de Clausura en Intersección LLC|los LLC no son cerrados en la intersección]]. Así que L puede no ser un LLC (si, por ejemplo los lenguajes son los del ejemplo de la otra demostración). Llegamos a una contradicción, que surge de asumir que los LLC son cerrados bajo la operación del complemento. 
Luego, los LLC no son cerrados bajo la operación de complemento.

***
#v2 
