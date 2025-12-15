#### Definición

Un lenguaje $Q\subseteq\Sigma_1^*$ es reducible a $L\subseteq\Sigma_2^*$ en [[Jerarquía de Velocidades de crecimiento|tiempo polinomial]], si existe una función total $f$, tal que:
- $f:\Sigma_1^*\mapsto\Sigma_2^*$ 
- $f\in\mathcal{O}(n^r)$
- $\forall w\in \Sigma_1^*: w\in Q ⇔ f(w)\in L$ 

![[Pasted image 20251209172821.png|500]]
- Similar al concepto de [[Reducción (de un problema A a un problema B)|reducción]] visto en [[Unidad 5 - Decidibilidad|computabilidad]] pero se incluye la restricción de la [[Complejidad Temporal de una MT|complejidad temporal]] de la función de transformación.

***
#### Teorema

Si $Q$ es un lenguaje reducible a $L$ en tiempo polinomial y $L \in\mathcal{P}$ , entonces $Q \in\mathcal{P}$
***
#### Uso
- Probar que algún problema es "tan difícil" de resolver como otros problemas cuya dificultad está probada.
- Mostrar que un problema no puede (hasta ahora) ser resuelto por un [[Algoritmo Eficiente]]
***
#### Etiquetas
- #Anki 