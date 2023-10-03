Create Project:
<br/>
Command: CREATE PROJECT test;<br/>
Result: Query successfully completed<br/>

Delete Project:<br/>
Command: DROP PROJECT test;<br/>
Result: Query successfully completed<br/>


List Project:<br/>
Command: SHOW [FULL] DATABASES
WHERE type = 'project';<br/>
Error: SQL statement cannot be parsed by mindsdb_sql - SHOW [FULL] DATABASES
WHERE type = 'project': Syntax error at token LBRACKET: "["
