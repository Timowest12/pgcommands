## Project Commands Collection

### Docker Commands

###### Pull PostgreSQL Image
	docker pull postgres

###### Run PostgreSQL Container
	docker run --name some-postgres -e POSTGRES_PASSWORD=secretpassword -d postgres

###### Bash into PostgreSQL Container
	docker exec -it some-postgres bash

### PostgreSQL Commands

###### Log into PostgreSQL(need to be in container)
	psql -U postgres

###### List All PostgreSQL Users
	\du

###### Create User with Password
	CREATE USER name WITH PASSWORD ‘secretpassword’;

###### Create User that Expires at Certain Moment
	CREATE USER name WITH PASSWORD ‘secretpassword’ VALID UNTIL '2005-01-01';

###### Create a Schema
	CREATE SCHEMA IF NOT EXISTS schema_name;
