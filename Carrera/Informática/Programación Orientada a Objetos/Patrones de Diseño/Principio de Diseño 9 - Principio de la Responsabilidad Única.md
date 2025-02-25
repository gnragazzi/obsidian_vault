Una clase debería tener solo una razón para cambiar.
***
Una clase debe hacer solo una cosa, y por lo tanto, tener una sola razón para cambiar.
***
En su forma más simple, pensá en una clase que maneja la lógica de presentación, de negocios y de persistencia. Esa clase podría cambiar en caso de que cualquiera de esos 3 aspectos cambie, indistintamente de si cambian todos. Para cumplir con este principio, deberíamos separar esa clase en 3.
***
Es un proceso que no se da únicamente en la fase de diseño, sino que se retroalimenta en cada etapa, cuando se observa que una clase cambia por mas de una única razón.
***
[[Cohesión]]