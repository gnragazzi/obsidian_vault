Datos en bruto para ser procesado por el cliente
Sin estado (misma llamada -> mismo resultado)
Se compone de
- Datos
- Componentes 
- Conectores (interfaces)
***
**RE**presentational **S**tate **T**ransfer

Es una [[API]] que cumple con 6 principios de diseño:
- Interfaz uniforme
	- Todas las solicitudes de API para el mismo recurso deben tener el mismo aspecto, sin importar de dónde provenga la solicitud.
- Desacoplamiento cliente-servidor
	- las aplicaciones de cliente y de servidor deben ser completamente independientes entre sí.
	- La única información que la aplicación de cliente debe conocer es el URI del recurso solicitado; no puede interactuar con la aplicación de servidor de ninguna otra manera. 
	- Del mismo modo, una aplicación de servidor no debe modificar la aplicación de cliente más que pasándole los datos solicitados a través de HTTP.
- Sin estado
	- Cada solicitud debe incluir toda la información necesaria para procesarla. Las API REST no requieren ninguna sesión del lado del servidor. 
	- Las aplicaciones de servidor no pueden almacenar ningún dato relacionado con una solicitud de cliente.
- Capacidad de almacenamiento en caché
	- Cuando sea posible, los recursos deben almacenarse en caché en el lado del cliente o del servidor.
- Arquitectura del sistema en capas
	- Las API REST deben diseñarse de modo que ni el cliente ni el servidor puedan saber si se comunica con la aplicación final o con un intermediario.