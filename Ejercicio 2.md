%basados_en_hechos_del_ejemplo
prop(donia_tota,madre,diego).
prop(don_diego,padre,diego).
%de_instanciacion
prop(diego,type,futbolista).
prop(lionel,type,futbolista).
prop(ayrton,type,automovilista).
prop(diego,type,campeon_mundial)
prop(diego,nacimiento,argentina).
prop(lionel,nacimiento,argentina).
prop(david,adopcion,francia).
%_de_herencia
prop(futbolista,subClassOf,deportista).
prop(automovilista,subClassOf,deportista).
prop(nacimiento,subClassOf,nacionalidad).
prop(adopcion,subClassOf,nacionalidad).


