@echo off
echo Connecting to MongoDB on AWS...

set HOST=3.25.100.10
set PORT=27017
set USER=admin
set PASS=MyPassword123
set AUTHDB=admin

"C:\Program Files\MongoDB\Server\6.0\bin\mongosh.exe" ^
--host %HOST% ^
--port %PORT% ^
--username %USER% ^
--password %PASS% ^
--authenticationDatabase %AUTHDB%

pause
