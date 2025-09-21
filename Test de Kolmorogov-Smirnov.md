#### Definición
- Compara la distribución de un conjunto de números generados con una distribución uniforme
#### Pasos
1. Ordenar los números aleatorios obtenidos de manera que $$R_1\le R_2\le ...\le R_n$$
2. Computar para 
	1. $D⁺=max_{(1\le i\le n) }\{\frac{i}{n}-R_i\}$  
	2. $D⁻=max_{1\le i\le n }\{R_i-\frac{i-1}{n}\}$  
3. Computar $D=max\{D⁺,D⁻\}$
4. Determinar el valor $D_\alpha$ para el nivel de significancia $\alpha$ y tamaño de muestra N (valores tabulados)
	1. Ejemplo![[Pasted image 20250920214845.png]]
5. Si $D \le D_\alpha$ se concluye que ninguna diferencia significativa fue detectada entre la distribución de $R_1\le R_2\le ...\le R_n$ y la distribución uniforme. Luego, la muestra se comporta como la distribución uniforme
	1. Caso contrario, la muestra se descarta.
***
#### Etiquetas
- #falta 