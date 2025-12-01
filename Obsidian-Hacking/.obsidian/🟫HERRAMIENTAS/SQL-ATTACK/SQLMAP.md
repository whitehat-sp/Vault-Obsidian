
Herramienta automatizada para la verificación de posibles inyecciones y explotación posterior en una web
# Repositorio
https://github.com/sqlmapproject/sqlmap

# EJECUCION

python3 sqlmap.py -u "http://"  --batch

python2 sqlmap.py -u "http://"  --batch


## Basic scan with crawling

 sqlmap -u "http://target.com" --crawl=3 --batch --forms

       --crawl=3: Crawls the website up to 3 levels deep  

       --batch: Never asks for user input, uses default responses  

       --forms: Automatically tests all forms found

## Scan request file

sqlmap -r login-request.txt --level=5 --risk=3 --batch

       --level=5: Most through testing level (default is 1)  

       --risk=3: Includes risky tests that could potentially cause problems (default is 1)