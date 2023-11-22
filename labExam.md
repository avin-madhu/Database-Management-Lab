# Lab Exam (Internal)

### Customer

| customer_id | first_name | last_name | age | country | 
| -------- | --------       | -------- |-----|---------|
| 1        | John         | Doe   |   31  |    USA     |
| 2        | Robert        | Luna   |   22  |   USA      |
| 3        | David        | Robinson   |   22  |   UK      |
| 4        | John         | Reinhardt  |    25 |      UK   |
| 5       | Betty        | Doe   |  28   |  USA      |



```
insert into Customers values(6, 'George', 'Bush', 46, 'USA')
```
After insert: 

| customer_id | first_name | last_name | age | country | 
| -------- | --------       | -------- |-----|---------|
| 1        | John         | Doe   |   34  |    USA     |
| 2        | Robert        | Luna   |   22  |   USA      |
| 3        | David        | Robinson   |   22  |   UK      |
| 4        | John         | Reinhardt  |    25 |      UK   |
| 5       | Betty        | Doe   |  28   |  USA      |
| 6       | George        | Bush   |  46   |  USA      |


```
delete from Customers where customer_id = '5'
```
After delete: 

| customer_id | first_name | last_name | age | country | 
| -------- | --------       | -------- |-----|---------|
| 1        | John         | Doe   |   31  |    USA     |
| 2        | Robert        | Luna   |   22  |   USA      |
| 3        | David        | Robinson   |   22  |   UK      |
| 4        | John         | Reinhardt  |    25 |      UK   |
| 6       | George        | Bush   |  46   |  USA      |


```
create table products (product_id int, name varchar(20), price int, shipping_id int);

insert into products (1, product1, 200, 2), (2, product2,250, 1), (3, product3, 350, 5), (4, product4, 150, 3);
```

| product_id | name | price | shipping_id | 
| -------- | --------| --------|-----|
| 1        | product1 | 200  |   2  |    
| 2        | product2 | 250  |   1  |  
| 3        | product3 | 350  |   5  |  
| 4        |product4  | 150  |    3 |     

```
ALTER TABLE Products
ADD PRIMARY KEY (product_id);
```























