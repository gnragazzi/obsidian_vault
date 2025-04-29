- Tenemos dos branches principales, que son estables y están protegidos:
	- Master
	- Develop
- Los nuevos desarrollos se trabajan desde branches que comiencen con nombre **feature/** y se abren pull request hacia **develop** para integrar
- Cuando se desea crear una versión a partir de develop se crea una branch **release** con el número de la versión que se desea crear. (por ejemplo, release/1.0.0)
- La versión y tag final se crea una vez que se realiza el merge del branch **release** a **master**
- En caso de existir un bug crítico, es posible crear un branch **hotfix/** directamente apuntando hacia master sin haber integrado a develop preciamente.
	![[Captura de pantalla 2025-04-28 a la(s) 4.05.58 p. m..png]]