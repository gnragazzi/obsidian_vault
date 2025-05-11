En el esquema tradicional, el proceso de selección de acciones (que tiene como resultado una *solución* al problema) se realiza *antes* de la ejecución de dichas acciones.
La certeza de este enfoque se da al considerar que las acciones que ejecuta el [[Agente Racional|agente]] son [[Ambiente - Agentes#^8f2617|deterministicas]], definiendo la función de transición $f$ como $$f: S × A \rightarrow S$$
Si bien este enfoque es apto para muchos problemas, no lo es en situaciones donde el agente **no tiene certezas sobre el efecto de sus acciones**. Esta [[Incertidumbre - IA|incertidumbre]] suele implicar la necesidad de **combinar** las observaciones que se tienen sobre el ambiente (dicho de alguna forma, el *feedback* del ambiente) con la ejecución de las acciones. Este tipo de problemas suele ser referenciado como *[[Problemas de contingencia]]*.
Luego, surge como alternativa para representar el no-determinismo de las acciones del agente reemplazando la función de transición como método de observar el efecto de las acciones del agente, por una [[Conceptos Probabilisticos ligados a IA|distribución de probabilidad]].
Las decisiones del ABU dependen de dos cosas fundamentales:
1. Lo que el agente ***cree***
	- Es la alternativa a "la verdadera realidad en el mundo", dada que esta es desconocida (en la mayor parte de los casos) por el agente. Es por esto que el agente debe *conformarse* con actuar basado en lo que cree
2. Lo que el agente ***desea***
	- Concepto más amplio que el de [objetivos] del agente, que implica considerar las *consecuencias* de que algo ocurra, como resultado de la acción.
La [[Teoría de la Decisión]] especifíca la forma de balancear la deseabilidad de los resultados con la probabilidad de que estos ocurran. Las utilidades obtenidas mediante una [[Función de Utilidad|función de utilidad]] son combinadas con las probabilidades para obtener la utilidad esperada de cada acción. 
***
[[Teoría de la Utilidad]]  

- 