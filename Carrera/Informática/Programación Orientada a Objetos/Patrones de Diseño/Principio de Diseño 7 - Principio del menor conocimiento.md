Habla solo con tus *amigos* más inmediatos. (También se conoce como la [[Ley de Demeter]])
***
Significa que al diseñar una clase hay que ser cuidadoso con la cantidad de clases con las que interactuamos y con cómo lo hacemos.
***
Cualquier método en un objeto solo debería llamar métodos que pertenezcan a:
- El mismo objeto
- Cualquier objeto pasado como parámetro
- Cualquier objeto que el método cree o instancie.
- Cualquier [[Composición - OOP|componente]] del objeto. [[Principio de Diseño 3 - Favorecer la composición a la herencia|Recordar este principio]]
En cualquier caso, no hay que llamar métodos que estén en un objeto que devuelva otro método (ver el ejemplo más abajo)
***
Este principio nos previene de diseñar sistemas con clases dependiendo de un montón de otras clases. Recordar que la [[Dependencia de Clases - OOP|dependencia]] se llama así porque si una clase cambia, esos cambios probablemente deban ser reflejados en la clase que depende de ella.
De esta manera, sistemas que tienen clases con múltiples dependencias son más frágiles y costosos de mantener.
***
![[Pasted image 20250213120838.png]]
***
Tener en cuenta que es un principio: seguirlo puede tener efectos en la performance de un sistema, por lo que debe ser usado con criterio.