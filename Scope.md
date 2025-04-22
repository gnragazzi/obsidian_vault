Llamamos Scope a la infraestructura que aloja nuestra aplicación.
![[Captura de pantalla 2025-04-21 a la(s) 7.43.04 a. m..png]]
- Instancia
	- Es la unidad mínima donde se aloja la aplicación.
- Cluster
	- Encargado del [[Escalamiento Horizontal]] 
- Load Balancer
	- Divide la carga entre las distintas instancias
***
Características
- Aplicación a la que pertenece
- Versión de la aplicación que está efectiva
- Tipo de cómputo standard o serverless
	- Standard está levantada todo el tiempo
	- Serverless es para procesos de prueba (no se mantiene levantado más de un tiempo x)
- Tipo de tráfico mess u off-mesh
- Provedor de cómputo
- 