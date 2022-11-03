# sql_server
SQL Server documentation

#Select processes under database

select * from sys.sysprocesses where dbid = DB_ID('database name')

#Drop database

USE master;
GO
alter database DatabaseProjectGlobalDatabase 
set single_user with rollback immediate
DROP DATABASE IF EXISTS DatabaseProjectGlobalDatabase;
GO
