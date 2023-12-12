### Create User with privileges

```
Create user 'username'@'localhost' identified by 'password';
```
```
Grant all privileges on *.* to 'username'@'localhost' with grant option;
```
Here Note that the first * indicates the `database` name and the second * indicates the `table` name.
```
Flush privileges;
```
### Some Common privileges

|Privileges| description|
|----------|------------|
|All privileges |The user is granted all privileges except GRANT OPTION and PROXY|
|ALTER     | The User can change the structure of the tables |
|CREATE   | The user can create databases and tables|
|DELETE    | The user can delete rows in a table |
|INSERT    | The user can insert values or rows in table |
|UPDATE    |The user can update rows in a table |
|SELECT    | The user can read rows from a table|

### Revoke Permissions
```
Revoke select, insert ON database_name.* from 'username'@'localhost';
```
