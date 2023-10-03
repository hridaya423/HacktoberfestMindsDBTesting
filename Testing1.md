List Data Handlers:<br/>
Command: SHOW HANDLERS
WHERE type = 'data';
<br/>
Result: Passed
<br/>

Connect a Data Source:
<br/>
Command:CREATE DATABASE mysql_datasource
WITH ENGINE = 'mariadb',
PARAMETERS = {
  "user": "root",
  "port": 3307,
  "password": "password",
  "host": "127.0.0.1",
  "database": "my_database"
};

<br/>
Result: Pass
<br/>

Remove a Data Source:
<br/>
Command: DROP DATABASE mysql_datasource;  
<br/>
Result: Pass
<br/>

List Datasources:
<br/>
Command: SHOW DATABASES;
<br/> 
Result: Pass
<br/>

Use a Datasource:
<br/>
Command: USE postgresql;
SELECT * FROM data.insurance;
<br/>
Result: pass
<br/>
