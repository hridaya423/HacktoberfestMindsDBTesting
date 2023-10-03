List Data Handlers:<br/>
Command: SHOW HANDLERS
WHERE type = 'data';
<br/>
Result: ![image](https://github.com/hridaya423/HacktoberfestMindsDBTesting/assets/66767013/6381ca11-18fd-4652-9b0d-2e8418b92ec1)

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
Result: ![image](https://github.com/hridaya423/HacktoberfestMindsDBTesting/assets/66767013/25ec1783-a782-47f2-b274-87aa583a4eea)

<br/>

Use a Datasource:
<br/>
Command: USE postgresql;
SELECT * FROM data.insurance;
<br/>
Result: pass
<br/>
