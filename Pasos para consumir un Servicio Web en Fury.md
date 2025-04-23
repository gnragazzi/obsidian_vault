1. Desde el menú de la izquierda iremos a Services > Web donde veremos un listado de servicios.
2. En la columna Cname dev access tendremos la URL.
3. Desde clientes como Postman, Curl, o Insomnia podremos hacer request a este dominio
   - No te olvides de incluir el token, o recibirás 401 Unauthorized!
   - Puedes obtener el token desde el menú desplegable de la izquierda, haciendo click en la huella dactilar.
4. Un ejemplo de request: `curl https://<cname>/ping -H 'X-Tiger-Token: Bearer 1234'`
