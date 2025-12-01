
Protocolo para obtener acceso remoto a otras maquinas

Protocolo Default: **22**

TIPO DE ALGORITMO
- ssh2-enum-algos

DETERMINA EL TIPO DE AUTENTICACION CON EL USUARIO
- ssh-auth-methods --script-args="ssh.user=xxx"

OBTENER LA CLAVE DE SSH DEL HOST
- ssh-hostkey --script-args ssh_hostkey=full