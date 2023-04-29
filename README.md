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
 
### Use to display a list of all users and their rights 
```sql
\du
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

 

