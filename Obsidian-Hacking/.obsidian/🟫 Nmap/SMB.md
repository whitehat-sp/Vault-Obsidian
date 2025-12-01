Protocolo usado por Windows para la comunicacion entre dispostivos e interocomuncacion entre equipos con el mismo sistema

Protocolo Defult: **445 / 339**

INFORMACION DEL PROTOCOLO

- smb-protocols -> Version del protocolo
- smb-security-mode -> Nivel de seguridad aplicado al smb
- smb-enum-sessions -> Enumeración de sesiones sobre smb
- 

*APLICANDO CREDENCIALES SOBRE LOS SCRIPT*

Argumento para añadir al usar usuarios,password o ficheros con su contenido -> **--script-args** **smbusername=xxx,smbpassword=xxx**

EJEMPLO DE USO
- smb-enum-sessions **--script-args** **smbusername=xxx,smbpassword=xxx** 
	- Enumeracion de sesiones
	
- smb-enum-domains --script-args: Enumeraciones de dominios
	
- smb-enum-groups: Enumeracion de grupos

- smb-enum-services: Enumeracion de servicios

- smb-enum-shares,smb-ls:  Enumeraciones de item compartidos mediante ese protocolo
