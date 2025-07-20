##### Paso previo

Sean $L_1$ y $L_2$ dos [[Lenguajes Libres de Contexto - LLC|LLC]] generados por $G_1=\langle N_1,\Sigma_1,P_1,S_1\rangle$ y $G_2=\langle N_2,\Sigma_2,P_2,S_2\rangle$, respectivamente. (Asumimos que $V_1∩V_2=\emptyset$, dado que al ser variables, si se da que 2 variables comparten el nombre (la letra que los identifica), se puede renombrar sin cambiar el lenguaje que genera la gramática y, por lo tanto, esta presunción no impone una restricción a $G_1$ o $G_2$).

###### Demostración

- Definamos $G=\langle N_1 \cup N_2 \cup \{S\},\Sigma_1 \cup \Sigma_2,P_1 \cup P_2 \cup\{S\to S_1S_2\},S\rangle$. 
- El símbolo distinguido inicia una derivación en ambas $G_1$ y $G_2$. 
- Una derivación de más a la izquierda, tiene la forma $$S\Rightarrow S_1S_2\Rightarrow^*uS_2\Rightarrow^*uv$$donde
	- $u\in L_1$
	- $v\in L_2$
- Luego, $L(G)\subseteq L_1L_2$ 
- Podemos observar que toda cadena en $L_1L_2$ puede ser escrita como $uv$, con $u\in L_1$ $v\in L_2$. Vemos que $S_1\Rightarrow_{G_1}^*u$ y $S_2\Rightarrow_{G_2}^*v$, puesto que $S\Rightarrow S_1S_2$, vemos que $L_1L_2\subseteq L(G)$. 
- $L(G)= L_1L_2$ 
***
#v2 
