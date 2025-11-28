#### Definición
- Es similar a una [[Máquina de Turing - Determinista|MT - Determinística]], a excepción de que la función de transición se define como $$\delta:Q×\Gamma\rightarrow2^{Q×\Gamma×\{I,D,N\}}$$
- Se mantienen las definiciones de [[Configuración - MT|configuraciones]] y [[Secuencia de Configuraciones de una MT Determinística|secuencia de configuraciones]].

*** 
#### Aceptación de la Cadena
- Si al menos una de las hojas de un [[Árbol de Secuencia de Ejecución - MT no Determinística]] es una configuración final, la cadena es aceptada.
	- ![[Pasted image 20250817213041.png|300]]
- Formalmente
	- Una cadena $x\in\Sigma^*$ es aceptada por una MT no determinística si y solo si existe una secuencia de movimientos a través de la cual se alcanza una configuración final, partiendo de una configuración inicial.

***
#### Etiquetas
- #Anki 