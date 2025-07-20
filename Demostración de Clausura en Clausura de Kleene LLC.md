##### Paso previo

Sean $L_1$ un [[Lenguajes Libres de Contexto - LLC|LLC]] generado por $G_1=\langle N_1,\Sigma_1,P_1,S_1\rangle$.
###### Demostración

- Definamos $G=\langle N_1 ,\Sigma_1 ,P_1 \cup P_2 \cup\{S\to S_1S | \lambda\},S\rangle$. 
- El símbolo distinguido puede generar un número arbitrario de cadenas $S_1$.
- En su lugar, cualquier palabra derivada desde $S_1$ está en $L_1$, por lo que el $L(G)=L_1^*$ 
- Como $G$ es una [[Gramáticas Libres del Contexto - GLC|GLC]], $L(G)$ es un LLC

***
#v2 
