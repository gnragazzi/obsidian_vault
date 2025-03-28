Framework de unit testing del ecosistema de Java.
[[Arquitectura de JUnit 5]] 
***
- Se tiene que emular la estructura del proyecto y, correspondiendo a la clase cuyos métodos se quieren probar, se crea una clase `<Classname>Test` 
- Hay anotaciones para indicar los tests, instrucciones previas y posterior a cada test.
	- @Test
		- Indica qué metodo se ejecutará como un test.
		- Recordar que en cada uno de estos métodos deben estar comtempladas [[Las 3 a's del Unit Testing|las 3 a's]].
	- @BeforeEach 
		- Instrucciones que se ejecutarán antes de cada una de las pruebas.
		- Puede ser importante para hacer un setup del ambiente en el que ocurriran cada una de las pruebas.
	- 
[[Anotaciones para JUnit]]
