Adjunta dinámicamente responsabilidades adicionales a un objeto.
Provee una alternativa flexible a la herencia como medio para extender funcionalidad.
***
- Esto se logra envolviendo un objeto con otro de la misma superclase para extender funcionalidad, de manera de delegar las partes de esa funcionalidad que ya se encuentran programadas, en lugar de reescribirlas
- El objeto decorador agrega su propia funcionalidad o bien antes o después de la delegación al objeto que envuelve el resto del trabajo.
- Claramente, el patrón usa herencia, pero lo importante es no heredar comportamiento. El comportamiento se transmite a través de la *composición*.
***
![[Pasted image 20250117125110.png]]
***
La implementación implica la asignación a un supertipo de un envoltorio concreto (o varios) envolviendo un componente concreto, por ejemplo
```
superclase i = new wrapper_a(
	new wrapper_b(...
		new componente_concreto()
	...)
)
```
- En esta implementación, y generalmente, el constructor del envoltorio debería tomar un parametro de la super_clase y asignarlo a una variable para tener siempre control sobre ese objeto.
***
Principios de diseño que aplica
- [[Principio de Diseño 5 - abierto'cerrado]]
***
[Head First Design Patterns]
