Partiendo de la [[Intersección de dos Eventos - Regla del Producto|regla del producto]], en la cual tenemos que$$P(A).P(B|A) = P(B) . P(A|B)$$
llegamos a la Regla de Bayes, la cual dice $$P(B|A)=\frac{P(B)P(A|B)}{P(A)}$$
***
La regla de Bayes ha sido usada en la IA en situaciones donde se tiene ciertas creencias previas sobre una **hipótesis** $\theta$, y que están expresadas por una distribución de probabilidades *a priori* $P(\theta)$, se tienen ciertos datos $D$ (o evidencia) y tambien un modelo de la probabilidad de que esos datos sean observados bajo las distintas hipótesis, $P(D|\theta)$, redefiniéndose el teorema de bayes con la nueva notación, como:
$$P(\theta|D) = \frac{P(D|\theta)P(\theta)}{P(D)}$$
y usándose la siguiente terminología para referenciar a los términos de la ecuación:
- $P(\theta)$: distribución a prior. 
	- Es la distribución probabilística que refleja y sintetiza el conocimiento previo (o inicial) sobre los valores que puede tener la hipótesis, antes de observar los datos.
	- Cuando no se tiene demasiada información inicial sobre las hipótesis, es usual usar *a priori*-s que asignan igual probabilidad a todos los valores posibles de la hipótesis.
- $P(D|\theta)$: la verosimilitud, es decir la plausibilidad de los datos, dados los distintos valores de la hipótesis.
- $P(\theta|D)$: la distribución *a posteriori*.
	- Es la distribución de probabilidad de las hipótesis, una vez que se han conocido los datos y las creencias sobre las hipótesis son actualizadas acorde a la regla de Bayes.
- $P(D)$ la evidencia. Es la probabilidad de observar los datos $D$ promediada sobre todas las posibles hipótesis. Puede considerársela una constante de normalización que se obtiene a partir de la siguiente fórmula:
	- $P(D)=\sum_{\theta_i \in \theta} P(D|\theta_i)P(\theta_i)$ 
***
Usando esta última ecuación, podemos actualizar la regla de bayes a su versión final:
$$P(\theta|D) = \frac{P(D|\theta)P(\theta)}{\sum_{\theta_i \in \theta} P(D|\theta_i)P(\theta_i)}$$