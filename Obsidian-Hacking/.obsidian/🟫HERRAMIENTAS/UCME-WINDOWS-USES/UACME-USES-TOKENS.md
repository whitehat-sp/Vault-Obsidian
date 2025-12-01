## IMPERSONATING TOKEN

Una vez conseguido acceso con meterpreter a la maquina

Verificar el usuario con el que estamos dentro y permisos con sus token relacionados

Command User -> getid
Permisos -> getprivs

Dentro de los permisos 'deberia' estar "SeImpersonatePrivilege"

- Vamos ha aprvecharnos de este permiso, usando la herramienta **incognito** dentro de meterpreter
	- Es importante recibir mensaje de confirmacion en la terminal
	- En caso de caerse la conexion por meterpreter, ejecutamos el exploit y despues cognitio nuevamente

- Listado de tokens -> list_tokens -u (token por usuario)
- Para usar el token
	- impersonate_token "token con permisos de administrador"
- Con esto ya tendremos acceso a la maquina como admin 
- Abrimos una shell remota para ejecutar en la maquina victima lo que necesitemos


Anexo a la info de Metasploit, [[create [[METASPLOIT]]
