# Data Definition Language
The data definition language allows you to define new tables and the relations between tables as well. You can use DDL commands to create new columns in your database and add constraints on the data that can be inserted into the database as well.

Creating tables in SQL is very simple we use the CREATE Command to indicate that we need to create something and then we specify what we're creating like a database or a table. If it's a table we also need to define it's columns and their data types when creating the table.

```SQL
CREATE TABLE demo(
 id int(32);
 name varchar(25);
 phone int(32);
)
```