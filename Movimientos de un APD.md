### Dependiente de la Entrada 

- Tiene en cuenta el símbolo corriente en la cinta de entrada.  
- Luego, una transición de este tipo tiene la siguiente forma:  
$$\delta(q, a, Z) = \{(p_1, \gamma_1), (p_2, \gamma_2), \ldots, (p_n, \gamma_n)\}$$donde:  
$$q \in Q, \, a \in \Sigma$$es el símbolo de la entrada, $Z \in \Gamma$ es el tope de la pila y finalmente, $p_i \in Q, \, \gamma_i \in \Gamma^*$ con $i = 1, 2, \ldots, n$.

***
### Independiente de la Entrada

- No se tiene en cuenta el símbolo corriente en la entrada, representa una transición espontánea.  
$$\delta(q, \lambda, Z) = \{(p_1, \gamma_1), (p_2, \gamma_2), \ldots, (p_n, \gamma_n)\}$$  
- Es decir, que no se mira el símbolo de la entrada para tomar una decisión y además la cabeza lectora no se mueve.

***
### Etiquetas
#v2 