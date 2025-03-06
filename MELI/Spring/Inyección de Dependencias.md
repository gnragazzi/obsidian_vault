Es un Patrón de Diseño, y una forma de implementar el [[Inversion of Control]].
***
Los objetos definen sus dependencias SOLAMENTE a través de
- Parámetros de constructor
- Argumentos a un [[Factory Method]]
- Propiedades que se establecen (setters) en las instancias de un objeto, ya sea que se creó con un constructor sin argumentos o que fue devuelto por un FM.
***
En Spring, el contenedor de IoC inyecta las dependencias cuando crea el Bean.
Esto lo hace con la anotación [[@Autowired]]