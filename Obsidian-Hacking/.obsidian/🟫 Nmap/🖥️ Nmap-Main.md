
![[images.jpg]]
## Sin Target

Parametros -> **sn -vv** 
- sudo **nmap -sn -vv 192.168.1.0/24**

## Recopilacio total 

### TCP
	- sU.Verificacion de trafico UDP
	- Pn. Simula que los host estan leventados
	- vv. Detalles de la ejecucion
	- T4. Agresividad en el ataque
		- T1 (Insane). Mas lento pero menos ruido en la red
		- T5. Mas rapido el scanner pero se genera mas trafico
	- p1-65535. Analisis de todos los puertos posibles
	- sV. Comprobacion de la version de los servicios
	- A . Informacion detalla del host ej: (sistema operativo, en servidores web similar a sitemap, verificacion de robots.txt..) 

Ejemplo de ejecucion : **sudo nmap -sS -Pn -sV -T4 -p1-65535 -vv -A "target" o "network/mask"**
### UDP
	- sU.Verificacion de trafico UDP
Para el caso del scaner con trafico UDP aplica los mismo flag 

ejecucion : **sudo nmap -sU -Pn -sV -T4 -p1-65535 -vv -A "target" o "network/mask"**

