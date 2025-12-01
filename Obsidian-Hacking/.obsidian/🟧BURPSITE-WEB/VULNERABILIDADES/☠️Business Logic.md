## Trust-Client

Verificar con el metodo POST  la posibilidad de alterar un valor enviado en la request

	-productId=1&redir=PRODUCT&quantity=1&price=13

Para este caso se ha modificado el precio del producto

## High Level Logic Vulnerability

Este fallo de seguridad pude ser explotable cuando no se hace una validación correcta de todos los datos que se envían en el POST

Ejemplo
- PRODUCTO (a) = 700€ 
- PRODUCTO(b)= 160€

En caso de no tener en cuenta los valores de ambos item y solo el total se puede modificar la petición de forma que se utilice como referencia el valor mas alto en formato negativo y se reste el item con valor mas pequeño

Item A ➡️ -700 / Item B: 160 x n (numero de veces necesario para poder llegar al valor que queramos)

-700 + (160x5) . Da como resultado un total de 100€ , en vez 860€ (en caso de hace la compra normal)

**Se juega con la lógica de los valores**

## **Inconsisten Security Controls**

Se debe a errores de implementación en cuanto al control de las cuentas

Como por ejemplo usar un link de registro y modificar el correo con el dominio usado por el equipo de administración del sistema para hacer modificaciones no autorizadas

