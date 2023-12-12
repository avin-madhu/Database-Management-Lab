
### Create a stored procedure to add a row to the table "College" with values

-- table --

Ans: 

change the delimiter: 

```
delimiter $$
```
create the procedure: 

```
create procedure add_row(IN College_id int(10), IN college_name varchar(20), IN address varchar(30))
     begin
     insert into college values (college_id, college_name, address);
     end $$
```
change back the delimiter : 

```
delimiter ;
```
call the procedure: 

```
call add_row(12934, "CEC", "Chengannur");
```
the new Table: 

-- table --



