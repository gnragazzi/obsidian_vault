```
prop(lemon_computer,has_logo,lemon_icon).
prop(lemon_computer,has_color,green).
prop(lemon_computer,has_color,yellow).
prop(laptop_lemon_10000,subClassOf,lemon_computer).
prop(laptop_lemon_10000,weight_kg,1.1).
prop(comp_2347,type,laptop_lemon_10000).

%definir_la_instanciación
instancia(X,Y):-prop(X,type,Y).
%definir_la_herencia
herencia(X,Y):-prop(X,subClassOf,Y).
herencia(X,Z):-prop(X,subClassOf,Y),herencia(Y,Z).

%definir_consultas
consultarPropiedad(X,P,V):-prop(X,P,V).
consultarPropiedad(X,P,V):-prop(Y,P,V),instancia(X,Y).
consultarPropiedad(X,P,V):-prop(Z,P,V),instancia(X,Y),herencia(Y,Z). %solo_hereda_propiedades_en_primer_nivel
```
***
[[Doctrina Prolog]]  