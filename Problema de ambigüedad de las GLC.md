#### Decidibilidad
- El problema de [[Ambigüedad en GLC|AMB]] en [[Gramáticas Libres del Contexto - GLC|GLC]] es [[Problemas No Decidibles|no decidible.]] 

***
#### Demostración

1. Suponer que AMB es decidible
2. Transformar una [[Instancia PCP]] $\langle A,B\rangle$ en una instancia $\langle G_{AB}\rangle$ de AMB
	1. [[Construir una GLC G_A y G_B a partir de las listas A y B]]
	2. [[Construir una GLC G_{AB} a partir de G_A y G_B]]
3. Demostrar que $\langle A,B\rangle$ tiene solución si y solo si $T(\langle A,B\rangle)=\langle  G_{AB}\rangle$ es ambigua.
	1. [[Si <A,B> tiene solución, entonces T(<A,B>)=<G_{AB}> es ambigua]]
	2. [[Si T(<A,B>)=<G_{AB}> es ambigua, entonces <A,B> tiene solución]]
4. Entonces se obtiene un algoritmo para decidir PCP --> Absurdo!
***
#### Etiquetas
- #Anki 