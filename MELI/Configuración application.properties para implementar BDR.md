spring.application.name=NOMBREDESUAPI
- MySql
```
spring.datasource.driverClassName=com.mysql.cj.jdbc.Driver
spring.jpa.database-platform=org.hibernate.dialect.MySQLDialect
#spring.jpa.hibernate.ddl-auto=create-drop

# CONNECTION
# Database's User & Password
#spring.datasource.username=root
#spring.datasource.password=SUPASSWORD

# URL & Name
#spring.datasource.url=jdbc:mysql://localhost:3306/NOMBREDEBD

# Me permite mostrar por consola todas las consultas SQL que hibernate realiza
#spring.jpa.show-sql=true

# Estas tres lineas son para levantar un archivo SQL : Ambiente local y Test, en Producción no va.
# Activa el uso de scripts SQL
#spring.sql.init.mode=always
# Donde se alojan los scripts SQL (Si se guarda directo en resources es asi el classpath)
#spring.sql.init.data-locations=classpath:Data.sql
# Inicializa o llama a los scripts SQL luego de creadas las tablas
#spring.jpa.defer-datasource-initialization=true

# ----------------------------------------|  H2-CO Configurations  |-------------------------------------------------- #
##Habilitar una consola dentro de la web de H2
spring.h2.console.enabled=true

## Dictaminar cual es el conector de la base de datos que vamos a usar
spring.datasource.driverClassName=org.h2.Driver
## URL & Name
spring.datasource.url=jdbc:h2:mem:ELNOMBREDELABD

## En que dialecto se van a convertir las instrucciones SQL
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
##create-drop, update, create, none
spring.jpa.hibernate.ddl-auto=create-drop

## Connection
## Database's User & Password
spring.datasource.username=sa
spring.datasource.password=1234



## Path Default localhost:8080/h2-console
spring.h2.console.path=/h2-console

## show querys on console
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
## naming
spring.jackson.property-naming-strategy=SNAKE_CASE

## Activa el uso de scripts SQL
spring.sql.init.mode=always
## Inicializa o llama a los scripts SQL luego de creadas las tablas
spring.jpa.defer-datasource-initialization=true
## Donde se alojan los scripts SQL (Si se guarda directo en resources es asi el classpath)
spring.sql.init.data-locations=classpath:Data.sql
```