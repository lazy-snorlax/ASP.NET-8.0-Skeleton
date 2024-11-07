# Test Stack for ASP.NET Core
This is a stack for local development with .NET 8.0 in a docker container. The ASP.NET project will fire up on http://localhost:8000. This project is primarily targeted for developing on Linux systems or for those without Visual Studio.

## Front End
Realistically, this service is completely optional. It is entirely possible to develop an application using only the .NET service, but for those who like to separate services (API, Frontend, Database) this is an example to follow. This service will fire up on http://localhost:8080.

Note: This was generated from the Vite init command, and does not mean that this should be locked into Vue only. Feel free to use React or any other frontend framework & libraries.

## MS SQL Database setup
In order for data to persist, you must create a db directory in the project root. Run these commands to create the sub-directories needed with the proper permissions for volume sharing the data with MSSQL.
```
mkdir data && sudo chown 10001 data
mkdir log && sudo chown 10001 log
mkdir secrets && sudo chown 10001 secrets
```
This service should start on http://localhost:1433.