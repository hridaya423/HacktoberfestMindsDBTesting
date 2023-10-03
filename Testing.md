Create Project:
Command: CREATE PROJECT test;
Result: Query successfully completed

Delete Project:
Command: DROP PROJECT test;
Result: Query successfully completed


List Project:
Command: SHOW [FULL] DATABASES
WHERE type = 'project';
Error: SQL statement cannot be parsed by mindsdb_sql - SHOW [FULL] DATABASES
WHERE type = 'project';
: Syntax error at token LBRACKET: "["
