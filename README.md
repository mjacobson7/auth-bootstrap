# auth-bootstrap

## Node, Express, & PostgreSQL

### To verify that you have the NodeJS, NPM and PostgreSQL installed on your PC, type the following commands on your command-line one after the other:

```
$ node --version

$ npm  --version

$ psql --version
```

### If you have their version printed, then you are Good to go. Create the database-user and the database for the application. Type the following on your command-line:

```
psql -c 'CREATE ROLE "postgres" with Login Superuser Createrole CreateDB Replication BypassRLS'
```

You need to create an equivalent database for postgres user before you can work with it.

```
psql -c 'CREATE DATABASE "postgres"'
```

and then create the database for the application:

```
psql -U postgres -c 'CREATE DATABASE "auth-system"'
```

Credit goes to: https://www.codementor.io/emjay/how-to-build-a-simple-session-based-authentication-system-with-nodejs-from-scratch-6vn67mcy3

