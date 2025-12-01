Herramienta utilizada para realizar fuerza bruta sobre una URL

Available Commands:
  completion  Generate the autocompletion script for the specified shell
  dir         Uses directory/file enumeration mode
  dns         Uses DNS subdomain enumeration mode
  fuzz        Uses fuzzing mode. Replaces the keyword FUZZ in the URL, Headers and the request body
  gcs         Uses gcs bucket enumeration mode
  help        Help about any command
  s3          Uses aws bucket enumeration mode
  tftp        Uses TFTP enumeration mode
  version     shows the current version
  vhost       Uses VHOST enumeration mode (you most probably want to use the IP address as the URL parameter)

## Ejecución

	- sudo gobuster dir -u https:// -w diccionario 
## Diccionario Ruta

Ruta por defecto de los diccionario 

	- usr/share/wordlist 
