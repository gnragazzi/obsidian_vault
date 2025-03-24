- HEAD
	- Devuelve la metadata del recurso que se hubiera obtenido con un método GET en la misma URL, en forma de [[Carrera/Informática/Lenguajes de Programación/Java/HTTP Header|headers]].
		- permite anticiparse a descargas costosas, ya que un campo del header es `content-length`
	- Si la respuesta al request muestra que una URL cacheada está desactualizada, se puede invalidar esa copia aun sin haber hecho un GET request.
- GET
- POST ^f966af
- PUT ^ed4ec5
	- Actualizar por completo un registro existente.
- PATCH ^eaa039
	- actualizar algún dato de un registro existente.
- DELETE
***
Patch y put son similares: ambos sirven para rectificar (UPDATE) información en el servidor.
![[Captura de pantalla 2025-02-28 a la(s) 3.36.35 p. m..png]]