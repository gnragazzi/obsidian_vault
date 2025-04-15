Es posible establecer variables de entorno con el comando de [[Bash]]
`export <nombre_variable>=<valor_variable>`
Estas variables pueden ser usadas dentro de un programa, utilizando la notación
`${<nombre_variable>}`
Esto es útli a la hora de configurar contraseñas, por ejemplo de la [[Configuración application.properties para implementar BDR|base de datos en la configuración de spring]].
***
Para que estas contraseñas persistan, es importante establecer ese comando en el archivo de configuración de la terminal, que puede ser:
`~/.bashrc`, `~/.bash_profile`, o `~/.zshrc`.