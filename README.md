# Test Stack for ASP.NET Core Dev
This is a stack for local development with .NET 8.0 in a docker container. The ASP.NET project will fire up on http://localhost:8000. This project is primarily targeted for developing on Linux systems or for those without Visual Studio.

## MS SQL Database setup
In order for data to persist, you must create a db directory in the project root. Run these commands to create the sub-directories needed with the proper permissions for volume sharing the data with MSSQL.
```
mkdir data && sudo chown 10001 data
mkdir log && sudo chown 10001 log
mkdir secrets && sudo chown 10001 secrets
```