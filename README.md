# crt
Continuous Recovery Testing for SQL Server

## What's this all about?
This project gives you procedures to test restores of SQL Server backups. The idea is to permanently check the restore of newly created backups by restoring them into a separate database (probably on a seperate instance of SQL Server). However the procedures can also be used for disaster recovery as they generate all the RESTORE commands for restoring a full set of backups.

## Prerequisites
* SQL Server 2008 - 2016 
* Backups created with the SQL Server Maintenance Solution from (https://ola.hallengren.com "Ola Hallengren")
* Option xp_cmdshell activated on the restore target server (setup script provided)
* XEvent Session for capturing errors ocurring during restore operations (setup script provided)

## License
All code written by Martin Guth has the CC BY-SA 4.0 license (https://creativecommons.org/licenses/by-sa/4.0/).
