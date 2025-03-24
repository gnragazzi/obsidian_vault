Un Java Bean es un estándar de definición de clases de negocio que tiene requisitos concretos.
- Las propiedades son privadas y tienen getters/setters públicos
- Debe tener un constructor público, sin parámetros
	- Esto no significa que no puede tener otros constructores, pero debe si o si implementar ese
- Debe implementar *Serializable*