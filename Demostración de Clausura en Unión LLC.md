##### Paso previo

Sean $L_1$ y $L_2$ dos [[Lenguajes Libres de Contexto - LLC|LLC]] generados por $G_1=\langle N_1,\Sigma_1,P_1,S_1\rangle$ y $G_2=\langle N_2,\Sigma_2,P_2,S_2\rangle$, respectivamente. (Asumimos que $V_1∩V_2=\emptyset$, dado que al ser variables, si se da que 2 variables comparten el nombre (la letra que los identifica), se puede renombrar sin cambiar el lenguaje que genera la gramática y, por lo tanto, esta presunción no impone una restricción a $G_1$ o $G_2$).
a
###### Demostración

- Definamos $G=\langle N_1 \cup N_2 \cup \{S\},\Sigma_1 \cup \Sigma_2,P_1 \cup P_2 \cup\{S\to S_1|S_2\},S\rangle$. 
- Una cadena $w\in L(G)$ si y solo si hay una derivación $$S\Rightarrow S_i\Rightarrow^*w$$para $i=1,2$. 
	- Luego, $w\in L_1 \lor w\in L_2$.
- Como $G$ es una [[Gramáticas Libres del Contexto - GLC|GLC]], $L(G)$ es un LLC

***
#v2 
