Aunque tanto [[ORM (Object-relational mapping)|ORM]] como [[DAO|DAO]] son patrones de diseño que se ocupan de tareas en la capa de persistencia de una aplicación, son cosas distintas.
- DAO es un patrón de diseño cuya principal función es establecer una interfaz normalizada para acceder a los datos, es decir que define un método de acceso a los datos, y operaciones que las realizan.
- ORM es un patrón de diseño que permite manipular los datos en una [[Base de Datos Relacional]] como si se tratara de objetos (en el caso, objetos java).
Amos patrones se pueden utilizar de manera conjunta, por ejemplo, usando el DAO como un punto de acceso a los datos, e implementando esas operaciones a través ORM.