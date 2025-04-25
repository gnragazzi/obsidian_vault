Las 3 partes, son:
- Producer
	- [[Generación de Mensajes - BigQueue ]]
	- Los mensajes pueden ser públicos o privados
- Topic
	- Broker
	- Realiza un HTTP POST para pasar la información a los consumidores. (comunicación tipo PUSH)
	- [[Características del Topic]] 
	- Puedo producir en tópicos de otra app (attach) con autorización del dueño
	- Puedo crear consumers de cualquier tópico (público) o de los de mi app
- Consumer
	- Los mensajes pendientes de procesar se llaman backlog o lag
	- [[Características del Consumer]] 
***
¿Cuando usarlo?
- Fuente de novedades hacia múltiples interesados (conocidos o no).
- Desacople de request con capacidad de procesarlo.
- Poder controlar picos de tráfico (buffer de olas de mensajes).
***
Garantías:
- NO garantiza el Orden.  
- No garantiza la Unicidad.  
- Al menos una vez se entrega el mensaje.  
- Se reintenta hasta que se entrega el mensaje o se cumple alguna estrategia de Error Handling.  
- Time to delivery (Midiendo consumers sin errores) - SLO WIP.
***
[[Buenas y Malas Prácticas - BigQueue]] 