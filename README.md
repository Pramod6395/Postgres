# Postgres

To connect to db in linux
```bash
psql -U <postgre username> 
psql -U <postgre username> -d <dbname>
```
List available databases
```bash
\l
```
Switch connection to a new database
```bash
\c <databaseName>
```
Check DB size in GB
```bash
SELECT pg_size_pretty( pg_database_size('dbname') );
```
To determine the size of a table in the current databas
```bash

SELECT pg_size_pretty( pg_total_relation_size('tablename') );
```
List available tables in db
```bash
\dt
```
Describe a table such as a column, type, modifiers of columns, etc.
```bash
\d <table_name>
```
Truncate table
```bash
TRUNCATE TABLE <tableName> ;
```
List all schemes of the currently connected database
```bash
\dn
```
List available functions in the current database
```bash
\df
```
List available views in the current database
```bash
\dv
```
List all users and their assign roles
```bash
\du
```
Retrieve the current version of PostgreSQL server
```bash
SELECT version();
```
Execute the last command again
```bash
\g
```
Display command history
```bash
\s
```
Save the command history to a file
```bash
\s filename
```
Execute psql commands from a file
```bash
\i filename
```
Know all available psql commands
```bash
\?
```
Get help
```bash
\h
```
Exit psql shell
```bash
\q
```
To beutify the query output with horizontal table formate 
```bash
\x on
```
DROP database
```bash
DROP DATABASE <dbname>
```
DROP database ForceFully Even session are active with users
```bash
DROP DATABASE <database name> WITH (FORCE);
```

