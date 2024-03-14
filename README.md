# Project Commands Collection

## Docker Commands

- **Pull PostgreSQL Image**
  \```shell
  docker pull postgres
  \```

- **Run PostgreSQL Container**
  \```shell
  docker run --name some-postgres -e POSTGRES_PASSWORD=secretpassword -d postgres
  \```

- **Bash into PostgreSQL Container**
  \```shell
  docker exec -it some-postgres bash
  \```

## PostgreSQL Commands

- **Log into PostgreSQL**
  \```sql
  psql -U postgres
  \```

- **List All PostgreSQL Users**
  \```sql
  \du
  \```

- **Create User with Password**
  \```sql
  CREATE USER name WITH PASSWORD ‘secretpassword’;
  \```

- **Create User that Expires at Certain Moment**
  \```sql
  CREATE USER name WITH PASSWORD ‘secretpassword’ VALID UNTIL '2005-01-01';
  \```

- **Create a Schema**
  \```sql
  CREATE SCHEMA IF NOT EXISTS schema_name;
  \```
