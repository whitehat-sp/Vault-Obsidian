
https://medium.com/@0xAwali/template-engines-injection-101-4f2fe59e5756

Vulnerabilidad con posibilidad de explotación dependiendo del motor de plantillas /templates usadas

La verificacion mas simples confirmar si gestiona correctamente la siguiente entrada

<mark style="background: #FFB86CA6;">{{7*/7}}</mark>

En caso afirmativo tocara verificar la tecnlogia que este usando

Una dato rapido es el host con el inspector una vez enviado el POST

F12 >Filtrar Cabeceras > Server: "<mark style="background: #BBFABBA6;">**información importante**</mark> 👀"

Posibles tecnologias

- PHP – Smarty, Twigs
- Java – Velocity, Freemaker
- Python – JINJA, Mako, Tornado
- JavaScript – Jade, Rage
- Ruby – Liquid

## jinja2 - Python

	-{{ self.__init__.__globals__.__builtins__.__import__('os').popen('id').read() }}

- El comando que se ejecutara en la maquina remota es lo que contiene después del .popen('<mark style="background: #ABF7F7A6;">comando_sistema</mark>')

