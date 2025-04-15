1. Crear la dependencia en el proyecto
```
<dependency>  
    <groupId>org.springframework.boot</groupId>  
    <artifactId>spring-boot-starter-data-elasticsearch</artifactId>  
</dependency>
```
2.  En el `application.properties` agregar 
```
spring.elasticsearch.uris=http://localhost:9200  
spring.elasticsearch.username=elastic  
spring.elasticsearch.password=
```

3. Anotaciones dentro de la entidad
```
@Document(indexName = "blog") //INDICA EL NOMBRE DEL ÍNDICE  
@Getter @Setter  
public class Article {  
    @Id // INDICA QUE ESTE CAMPO SERÁ USADO COMO IDENTIFICADOR UNÍVOCO  
    private int id;  
    private String title;  
  
    @Field(type = FieldType.Nested, includeInParent = true) //INDICA QUE ESTE CAMPO ESTARÁ ANIDADO DENTRO DE ARTICULO  
    // (se utiliza para definir un objeto JSON que conserva la relación con sus subcampos.)    private List<Author> authorsList;  
  
}
```