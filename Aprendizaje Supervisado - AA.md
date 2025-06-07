## Definición Formal
La experiencia de entrenamiento es un conjunto de ejemplos $$\langle\vec{x},o(\vec{x})\rangle$$donde:
- $\vec{x}$ = representación (vectorial) de algún objeto (imagen, texto, etc).
- $o(\vec{x})$ = clase/categoría o valor numérico asociado a $\vec{x}$. 
***
### Idea Intuitiva
- intentar reproducir un proceso de clasificación correcto/ideal ($clasificador_{ideal}$ )
- que para cada entrada (el objeto que se quiere clasificar) o, genera una salida c (la clase de o)
- Luego, usando ejemplos $〈o, c〉$ del comportamiento de $clasificador_{ideal}$, entrenar otro clasificador ($modelo$) cuyos comportamientos sean tan parecidos como sea posible.
	- ![[Pasted image 20250607132043.png]]
Las salidas del modelo deberían corresponderse con las del clasificador ideal en:
- Datos de entrenamiento
- en datos no vistos anteriormente (**generalización**)
	- Esto se conoce como Aproximación de una Función
Este proceso se llama [[Aprendizaje de un Clasificador-Hipótesis]] 
***

***
## ¿Qué tipo de modelos se aprenden?

- Predictivos
***
## [[Flujo del Aprendizaje Automático]]  
