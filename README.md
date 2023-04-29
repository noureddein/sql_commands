## SQL commands

### Start Using PostgreSQL 
```sql
sudo -u postgres psql
```
	
### To login to postgres and database:
- To login in to postgres with user:
```sql
sudo su - <username>
```
- Then login in to the database:
```sql
psql
```

### list of all the databases that are available on a server
```
\l
```
 
### Use to display a list of all users and their rights in the current database server
```sql
\du
# OR
\du+
```
 	
### To set the password for a user
```sql
# You should be logged in to the database and have all roles to edit user

\password postgres
```

### To create a user with password
```sql
create user <username> with password '<password>';
```
 
### To create new database
```sql
CREATE DATABASE <database_name>;
```
### To give privileges on a database for specific user:
```sql
grant all privileges on database <database_name> to <username>;
```

### connect to database with user
```sql
psql -h localhost -d postgres -U <username>
```

### To start database
```sql
sudo service postgresql start
```
### Display information about current connection
```sql
\conninfo              
```

### TO ALTER A USER ROLES
https://www.postgresql.org/docs/9.2/sql-alterrole.html
```sql
ALTER ROLE <username> <role_name>;  
```

### LIST ALL DATABASES
```sql
\l 				        => list databases with there users
\l+ 				    => list databases with more informations
\db <database_name>  	=> This will display information about the tables, functions, and other objects in the database.
```


