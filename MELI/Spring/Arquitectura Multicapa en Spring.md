Un servidor implementado en [[Carrera/Informática/Lenguajes de Programación/Java/Spring|Spring]] consta de 5 capas (puede variar).
- Capa de interfaz (Controller) ^2357da
	- Atiende la solicitud y entrega la respuesta
	- @RestController
- Capa de negocio (service)
	- Se encarga de contener la lógica de negocio de la aplicación. Debe marcarse con @Service
- [[Data Transfer Object Pattern (DTO)]]
	- Conjunto de datos planos que se utilizan para interacción entre cliente y servidor y sirve para esconder la representación de datos, desacoplar request/response de la representación de datos y evitar redundancia o exceso de datos.
	- Existen DTOs de request y DTOs de response
- Capa de acceso a datos Repository (DAO)
		- Es la capa de persistencia de datos. Cada clase de repositorio debe estar marcada con la anotación @Repository
		- encapsula el comportamiento de almacenamiento, recuperación y búsqueda
- Capa de Infraestructura
	- Base de datos (entity)
		- Tabla almacenada en una base de datos. Cada instancia de una entidad es una fila en una tabla. Las clases-entidad deben estar marcadas con @Entity
		- También llamada model
	- ![[Captura de pantalla 2025-03-05 a la(s) 3.41.17 p. m..png]]
	- Observar la relación con [[MVC|MVC]]
***
La arquitectura debe verse reflejada en el árbol del proyecto.
![[Captura de pantalla 2025-03-05 a la(s) 3.45.38 p. m..png]]
Es importante recordar que distintas carpetas = distintos paquetes.
Esta división parece más significativa: cada capa tiene su propio paquete (llamado igual que la capa). Así, si quiero encontrar una entidad, por ejemplo, se en qué capa debo buscarla.
***
En la capa de servicio (y asumo que en todas las capas) se deben construir interfaces e implementarlas, como forma de desacoplar la implementación.