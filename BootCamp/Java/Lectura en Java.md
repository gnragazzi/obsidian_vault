Lo principal es crear una instancia de la clase Scanner, con `System.in` como argumento:
```
Scanner teclado = new Scanner(System.in);

int num = teclado.nextInt();
String nombre = teclado.next();
double promedio = teclado.nextDouble();
```