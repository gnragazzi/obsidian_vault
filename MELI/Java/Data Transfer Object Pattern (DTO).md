La finalidad de este patrón de diseño es crear un objeto plano ([[POJO]]) con atributos que puedan ser enviados o recuperados del servidor en una sola invocación.
***
- Separar las estructuras de datos del modelo de datos.
- Controlar el formato de los datos a almacenar dentro del modelo de datos.
***
En el bootcamp, 
- El DTO es un objeto JAVA utilizado para la transferencia de la información.
- Es inmutable
- Sirve para mappear varias entidades en un único objeto plano que se devuelve
- Solo debe tener los métodos getter y setter
- Debe implementar [[Serializable JAVA]]
- Deben utilizarse RequestDTO y ResponseDTO
***
![[Captura de pantalla 2025-03-05 a la(s) 3.12.20 p. m..png]]