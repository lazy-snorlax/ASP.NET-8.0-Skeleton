# Test Stack for ASP.NET Core Dev

## MS SQL Database setup
In order for data to persist, you must create a db directory in the project root. Run these commands to create the sub-directories needed with the proper permissions for volume sharing the data with MSSQL.
```
mkdir data && sudo chown 10001 data
mkdir log && sudo chown 10001 log
mkdir secrets && sudo chown 10001 secrets
```