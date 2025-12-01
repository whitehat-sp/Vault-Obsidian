Para la ejecucion de estos modulo, sera necesario tener una sesion de meterpreter previamente 

[*]use post/windows/gather/win_privs[*]
	Comprueba los 

[*]use post/windows/gather/enum_logged_on_users[*]
	-Comprueba los usuarios logueados en el servidor

[*]use post/windows/gather/checkvm[*]
	-Comprueba si la maquina destino es una maquina virtual

[*]use post/windows/gather/enum_applications[*]
	-Comprueba las aplicaciones o programas instalados en la maquina

[*]use post/windows/gather/enum_patches[*]
	-Comprueba los KB instalados en la maquina destino

[*]use post/windows/gather/enum_shares[*]
	-Comprueba los objetos compartidos mediante el protocolo SMB
	