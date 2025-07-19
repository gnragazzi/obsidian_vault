La idea es expresar la granática en forma iterativa, utilizando [[BNFE]]. 
Es posible utilizar la factorización, como se observa en el siguiente ejemplo:
- $Z→aZ|bZ|a|b$
- BNFE → $<Z>::= (a|b)\{(a|b)\}^*$ 
  #v2 