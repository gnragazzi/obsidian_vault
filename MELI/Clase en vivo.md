- Usar ModelMapper en lugar de ObjectMapper
	- Hay que agregar la dependencia 
```
<dependency>  
    <groupId>org.modelmapper</groupId>  
    <artifactId>modelmapper</artifactId>  
    <version>3.2.2</version>  
</dependency>
```

- Se puede utilizar un archivo de configuración para crear una versión singleton del modelMapper
	- Sería un archivo cualquiera, con una clase decorada con el anotador @Configuration y adentro un @Bean que tiene un método que devuelve un mismo modelMapper.![[Captura de pantalla 2025-04-11 a la(s) 11.59.33 a. m..png]]