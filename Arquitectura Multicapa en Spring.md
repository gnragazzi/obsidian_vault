Un servidor implementado en [[Spring]] consta de 5 capas (puede variar).
- Capa de interfaz (Controller)
	- Atiende la solicitud y entrega la respuesta
	- @RestController
- Capa de negocio (service)
	- Se encarga de contener la lógica de negocio de la aplicación. Debe marcarse con @Service
- Capa de Acceso a datos
	- [[Data Transfer Object Pattern (DTO)]]
	- Repository (DAO)
		- Es la capa de persistencia de datos. Cada clase de repositorio debe estar marcada con la anotación @Repository
		- encapsula el comportamiento de almacenamiento, recuperación y búsqueda
- Capa de Infraestructura
	- Base de datos (entity)
		- Tabla almacenada en una base de datos. Cada instancia de una entidad es una fila en una tabla. Las clases-entidad deben estar marcadas con @Entity
	- ![[Captura de pantalla 2025-03-05 a la(s) 3.41.17 p. m..png]]
***
La arquitectura debe verse reflejada en el árbol del proyecto
![[Captura de pantalla 2025-03-05 a la(s) 3.45.38 p. m..png]]
***
En la capa de servicio (y asumo que en todas las capas) se deben construir interfaces e implementarlas, como forma de desacoplar la implementación.