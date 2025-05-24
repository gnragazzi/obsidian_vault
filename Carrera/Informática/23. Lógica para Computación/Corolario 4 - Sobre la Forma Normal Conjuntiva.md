Toda [[Fórmula Lógica|fórmula]] que no sea [[Tautología, Contradicción y Contingencia|tautología]] es lógicamente equivalente a una fórmula restringida de la forma:
$$(\wedge^m_{i=1}(\vee^n_{j=1}Q_{ij}))$$
siendo cada $Q_{ij}$ una [[Variables Proposicionales|variable proposicional]] o la negación de una variable proposicional. Esta forma se  llama ***forma normal conjuntiva***.
***
_Demostración:_ Sea $P$ una fórmula que no es tautología. Entonces $\neg P$ no es contradicción y por el Corolario 3 sabemos que es lógicamente equivalente a una fórmula en forma normal disyuntiva:
$$\left( \bigvee_{i=1}^{m} \left( \bigwedge_{j=1}^{n} Q_{ij} \right) \right)$$
Luego $P$ es lógicamente equivalente a$$\neg \left( \bigvee_{i=1}^{m} \left( \bigwedge_{j=1}^{n} Q_{ij} \right) \right)$$y por las leyes de De Morgan, esto es lógicamente equivalente a
$$\left( \bigwedge_{i=1}^{m} \left( \bigvee_{j=1}^{n} \neg Q_{ij} \right) \right)$$
Finalmente una fórmula equivalente a $P$, escrita en forma normal conjuntiva, se obtiene reemplazando en esta fórmula cada expresión de la forma $\neg \neg q$ por $q$.
***
![[Captura de pantalla 2025-03-31 a la(s) 4.12.03 p. m..png]]![[Captura de pantalla 2025-03-31 a la(s) 4.12.14 p. m..png]]$