### Database version
        SELECT * @@version;

      ### Data directory location
        SELECT * @@datadir;

      ### Server hostname
        SELECT * @@hostname;

      ### Plugin directory location
        SELECT @@plugin_dir;

      ### Current database user
        SELECT * USER();

      ### Current system user
        SELECT CURRENT_USER();

      ### Time delays
        SELECT SLEEP(10)

      ### Listado de tablas
        SELECT * FROM information_schema.tables

      ### Listado de columnas
        SELECT * FROM information_schema.columns WHERE table_name = 'TABLE-NAME-HERE'

    ## Privilege escalation

      ### List user privileges
        SELECT grantee, privilege_type FROM information_schema.user_privileges;
      ### List user credentials
        SELECT host, user, authentication_string FROM mysql.user;