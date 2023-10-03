Command: CREATE PROJECT test;
Result: Query successfully completed

Command: DROP PROJECT test;
Result: Query successfully completed

Command: SHOW [FULL] DATABASES
WHERE type = 'project';
Error: SQL statement cannot be parsed by mindsdb_sql - SHOW [FULL] DATABASES
WHERE type = 'project';
: Syntax error at token LBRACKET: "["
