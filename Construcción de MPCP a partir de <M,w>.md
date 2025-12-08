Sea $M=\langle \Sigma,\Gamma,Q,\delta,q_0,q_f\rangle$ una [[Máquina de Turing Determinista - MT (MTD)|MTD]] y $w\in\Sigma^*$ que cumple con jamás "carse" por izquierda y no escribir blancos ($\mathbb{B}$). Construimos una [[Instancia MPCP]] a partir del par $\langle M,w\rangle$ de la siguiente manera:
1. 

| A         | B          | Explicación                           |
| --------- | ---------- | ------------------------------------- |
| $\#$      | $\#q_0w\#$ | (1)                                   |
| $\#$      | $\#$       | (2)                                   |
| $X$       | $X$        | (2) para cada $X\in\Gamma$            |
| $qX$      | $Yp$       | (3) si $\delta(q,X)=(p,Y,R)$          |
| $ZqX$     | $pZY$      | (3) si $\delta(q,X)=(p,Y,L)$          |
| $q\#$     | $Yp\#$     | (3) si $\delta(q,\mathbb{B})=(p,Y,R)$ |
| $Zq\#$    | $pZY\#$    | (3) si $\delta(q,\mathbb{B})=(p,Y,L)$ |
| $Xq_fY$   | $q_f$      | (4)                                   |
| $q_fY$    | $q_f$      | (4)                                   |
| $Xq_f$    | $q_f$      | (4)                                   |
| $q_f\#\#$ | $\#$       | (5)                                   |
dónde:
- $Z\in \Gamma$
- $q\in Q - \{q_f\}$ 
- $p\in Q$

***
#### Etiquetas
#Anki  