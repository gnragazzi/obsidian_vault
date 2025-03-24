Es una clase parametrizada 
```
ResponseEntity<T>
```
que nos permite un mayor control de qué se devuelve al cliente a partir de un [[Carrera/Informática/Lenguajes de Programación/Java/API REST y Spring#^c0241c|@GetMapping]] 
***
El constructor de ResponseEntity nos permite agregar [[Carrera/Informática/Lenguajes de Programación/Java/HTTP Header|headers]], los cuales pueden ser creados aprovechando la clase ***HttpHeaders***.
***
También se puede usar las clases anidadas para simplificar la creación del ResponseEntity
```
ResponseEntity.ok(<respuesta>) // automáticamente manda con status code 200
```

```
ResponseEntity.status(<numero_de_estado>).body(<cuerpo de la respuesta>)
```
***
Es una alternativa a `HttpServletResponse`, que puede ser dispuesta con métodos como `setHeader`, `setStatus`, etc...