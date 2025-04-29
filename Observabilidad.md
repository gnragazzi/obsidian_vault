Propiedad de los sistemas.
Un sistema es observable si su estado actual se puede determinar en un período de tiempo finito utilizando solo las salidas del sistema.
***
Los datos de telemetría no son observabilidad, sino que hay que instrumentar la recopilación de datos de telemetría usando [[MELT]]:
- Metrics
	- Mediciones cuantitativas
		- Tráfico,
		- Uso de cpu
- Events
	- Deploy
	- Ejecución de un comando
- [[Logs]] 
	- Exponer información interna
- Tracing
	- Origen del problema
***
Por ejemplo, usar tags para darle valor a los logs