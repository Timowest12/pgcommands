## Project Commands Collection

### Docker Commands

###### Pull PostgreSQL Image
	docker pull postgres

###### Run PostgreSQL Container
	docker run --name instance-name -e POSTGRES_PASSWORD=secretpassword -d postgres

###### Bash into PostgreSQL Container
	docker exec -it some-postgres bash

### PostgreSQL Commands

###### Log into PostgreSQL(need to be in container)
	psql -U postgres

###### List All PostgreSQL Users
	\du

###### Create User with Password
	CREATE USER username WITH PASSWORD 'secretpassword';

###### Create User that Expires at Certain Moment
	CREATE USER name WITH PASSWORD 'secretpassword' VALID UNTIL '2005-01-01';

###### Drop a user
	DROP USER IF EXISTS username;

###### Create a Schema
	CREATE SCHEMA IF NOT EXISTS schemaname;

###### Drop a Schema
	DROP SCHEMA IF EXISTS schemaname;

###### List all schemas
	select nspname from pg_catalog.pg_namespace;
 
