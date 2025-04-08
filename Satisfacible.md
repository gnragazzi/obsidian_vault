Una fórmula se dice ***satisfacible*** si existe una [[Función de Valuación Booleana|valuación]] que la [[Valuación que Satisface a una Fórmula|satisfaga]]. Caso contrario se dice ***insatisfacible***.
***
1. Toda valuación $v$ satisface (trivialmente) al conjunto vacío.
2. Un [[Conjuntos|conjunto]] finito y no vacío de fórmulas es satisfacible si y sólo si la conjunción de las fórmulas que lo componen es satisfacible. Sea $S=\{Q_1,Q_2,...,Q_n\}$ entonces:$$S\text{ es satisfacible si y solo si para alguna valuación $v$ tenemos que }v(Q_1∧Q_2∧...∧Q_n)=⊤$$
3. Una fórmula $P∈Form$ tal que $var(P)=\{x_1,x_2,...,x_n\}$ es satisfacible si y sólo si existe una $n$-upla $(a_1,a_2,...,a_n)∈B^n$ tal que $T_p(a_1,a_2,...,a_n)=⊤$.
4. Es claro que una fórmula es satisfacible si y sólo si es una [[Tautología, Contradicción y Contingencia|tautología]] o una contingencia.  Luego, las fórmulas insatisfacibles coinciden con las contradicciones (o falsedades).
***
[[Procedimiento para determinar si una fórmula es o no satisfacible]] 