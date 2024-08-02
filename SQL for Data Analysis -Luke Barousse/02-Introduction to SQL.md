# Introduction to SQL

Accessing and managing data and even the databases them selves in a relational database system is done through SQL a specialized programming language that is made specifically for relational databases.

Any command that we run in SQL to interact with the database is known as a query. Queries can perform CRUD operations on the data as well as create new databases and tables for us as well.

- CREATE or INSERT INTO statements in SQL allow us to create table or insert data into them respectively.
- SELECT statements allows to retrieve the data stored in the database.
- UPDATE statements allows to update tables or records in a table
- DELETE or DROP statements allows to remove data inside a table or the whole table itself respectively.

Relational databases are transaction based databases where changes won't occur at all if the query hasn't been run successfully and are mostly used in scenarios where all the data being stored is in a structured format. Like a job listing platform or a bike selling showroom.

SQL queries can be written in the query editor that your database provider provides you with or a cloud based editor if you're accessing your databases stored in a server or even a code editor like VSCode with the proper extensions so that it can connect to the database easily.

## Relational Databases

Popular SQL Databases like PostgreSQL and MYSQL provide you with their own editors like PGAdmin and PHPMyAdmin respectively. Cloud providers such as GCP and AWS also provide you their own editors in their cloud consoles that you can use to interact with the databases that you have stored on their servers.

There are multiple different SQL-based databases such as SQLite, PostgreSQL, MYSQL, and others and they all have the same tables and columns support but the syntax in which you write SQL queries is different for each of them.

There aren't any major changes that might affect your work but some built-in functions have a different syntax and some of them have more built-in features than others.