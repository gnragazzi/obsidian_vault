Se manejan a través de [[MELI/Spring/HTTP Response|HTTP Responses]]. Puede que, además de un mensaje, necesitemos enviar un JSON con información.
***
Hay 3 formas de manejar excepciones en [[MELI/Spring/Spring|Spring]], que se diferencian por los distintos casos en que son útiles, y por las anotaciones que son necesarias para utilizarlas:
- [[@ResponseStatus]]
- [[@ExceptionHandler]] 	
- [[@ControllerAdvice]] 