## Indexes

Indexes are used to retrieve data from the database more quickly than otherwise. The users cannot see the indexes, they are just used to speed up searches/queries.

### Basic Syntax: 

```
create index index_name
on table_name (column_1, column_2);

```

### Example: 

create an index on all the coloumn in the table "book"

| title            | author              |
|------------------|---------------------|
| The Catcher      | J.D. Salinger       |
| a Mockingbird    | Harper Lee          |
| 1984             | George Orwell       |
| The Great Gatsby | F. Scott Fitzgerald |
| The Catcher      | J.D. Salinger       |
| a Mockingbird    | Harper Lee          |
| Animal Farm      | George Orwell       |
| Half Girlfriend  | Chetan Bhagat       |
| Richer           | downy sprouse       |

```
create index book_index
on book (title);
```

### showing the index

```
show indexes on book;
```
here book is the table name.




