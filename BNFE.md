Versión extendida de [[BNF]] para facilitar la escritura y lectura
- Si un elemento es opcional se encierra entre .  
    Ejemplo:  
    `<selec> ::= if(<exp>) <sent> [else <sent>]`
- Para la elección de alternativas se usa `|` y opcionalmente también se pueden usar `()`.  
    Ejemplo:  
    `<for> ::= for <var> := <expresion> (to | downto) <expresion> do <sentencia>`
- Una secuencia arbitraria se encierra entre { }.  
    Ejemplo:  
    `<lista-ident> ::= <identificador> \{, <identificador>\}`