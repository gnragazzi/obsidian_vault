Es un espacio creado por Spring en tiempo de ejecución, en el que se agrupan instancias de objetos, llamados [[Beans - Spring|Beans]], para ser usadas en otro lugar de la aplicación.
El mecanísmo para hacer uso de un Bean se llama [[Inyección de Dependencias]] y es posible mediante [[MELI/Spring/Anotaciones de Spring Boot|anotaciones]].
***
La interfaz `org.springframework.context.ApplicationContext` representa el contenedor de Inversión de Control y es responsable de crear instancias, configurar y ensamblar los beans. Obtiene sus instrucciones leyendo los metadatos de configuración, en XML (en el POM?) o a través de anotaciones.
***
[[Principio de Diseño 8 - Principio Hollywood]] 