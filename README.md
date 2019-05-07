# REST API for PostgreSQL database

The application serves a REST API for a PostgreSQL database using Node.js 

## Getting Started

### Prerequisites

[npm](https://www.npmjs.com/)

[PosgreSQL](https://www.postgresql.org/)

### Installing

The dependicies can be resolved using 

```
npm init
```
## Deployment

Make the necessary changes to postgresql/config.json for database credentials.

```
{
  "port": 9999,
  "type": "postgresql",
  "db": {
    "server": "localhost",
    "user": "postgres",
    "password": "password",
    "database": "testing",
    "options": {}
  }
}
```

Make to following changes to postgresql/config.json for deplying on a server.

```
"server":"0.0.0.0"
```
Make the address 0.0.0.0 instead of localhost

## Running

Before running the app, make sure the PostgreSQL service is running.

then execute 

```
node postgresql/server.js 
```
By default, the app listens on port 9999.

## Built With

* [resquel](https://github.com/formio/resquel) - An express library
