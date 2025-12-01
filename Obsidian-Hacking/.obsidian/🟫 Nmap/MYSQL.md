Servicio usado por este tipo de BBDD

Default Protocol =  1433

#### OBTENER INFORMACION #### 

- ms-sql-info -> Informacion del protocolo
- ms-sql-ntlm-info --script-args mssql.instance-port=1433 -> Info NTLM
- ms-sql-empty-password -> Verificacion de usuarios con contraseñas vacias

APLICANDO CREDENCIALES SOBRE LOS SCRIPT

Argumento para añadir al usar usuarios,password o ficheros con su contenido -> **--script-args** **smbusername=xxx,smbpassword=xxx**

EJEMPLO 
- ms-sql-brute --script-args userdb=diccionario_user,passdb=diccionario_passwords

- ms-sql-dump-hashes: Dumpeo de hashes de los usuarios
- ms-sql-xp-cmdshell: Ejecucion remota de comandos sobre el servidor
	- Para el caso de este script se tendra que añadir un 3º paramatro, donde se indica el comando a ejecutar de manera remota
		- ms-sql-xp-cmdshell.cmd="comando-a-ejecutar"
