# docker-postgresql

## Description

This is container of postgreSQL for develop backend service in local environment.

## How to use
### 1. Create `.env`
```
POSTGRES_USER=USER_NAME_HERE
POSTGRES_PASSWORD=PASSWORD_HERE
POSTGRES_DB=DB_NAME_HERE
```

### 2. Set up initial sql at `setup.sql`

### 3. Connect outside form container
```
psql -h localhost -p 8090 -U USER_NAME_DEFINED_in.env
```

or from another container
```
psql -h sample-postgres -U USER_NAME_DEFINED_in.env
```
