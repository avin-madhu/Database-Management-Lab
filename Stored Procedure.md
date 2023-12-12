### Stored Procedures

 Stored Procedures allows you to group and encapsulate a series of SQL and procedural statements, making it reusable.

consider the table below named 'college'

| college_code | college_name | address           |
|--------------|--------------|-------------------|
|        12982 | TKM          | Kollam            |
|        12983 | RIT          | Pambady, Kottayam |
|        12986 | CET          | Trivandrum        |
|        12988 | GEC          | Trissur           |


we can display the details of the table using store procedure: 

basic syntax: 

```
    create procedure get_college()
    begin
        -- sql query --
    end 
```

NOTE: 
usually in a query the query ends with ';' we don't want that as the stored procedure syntax ends there and we can't proceed further
to write the 'end' 
hence we change the delimiter to '$$' instead of ';' (you can change it to any character)
Hence we can write the stored procedure as: 
```
   delimiter $$
   create procedure get_college()
    begin
        select * from college;
    end $$
```
Here the statements end at "...end $$ " instead of "...college; " 
    
NOTE: 
change the delimiter back to ';' using: 
```
delimiter ;
```



