# Introduction to PostgreSQL
PostgreSQL is the most widely used and advanced open-source SQL based relational database solution. It provides a solid stability, security, and scalability features that make it a great choice for enterprise level systems.

PostgreSQL is mainly a SQL based relational database management system but has a great community of developers that have developed extensions and tools for it so that it can be used with different types of data and use cases such as geo-spatial and time series data.

## Unlimited power
Postgres is a relational database management system that uses SQL as it's main programming language. A single instance of postgres can store up to 4 billion individual databases each with a billion tables and rows.

> The amount of databases and tables stored in an instance is dependent on the configuration of the server that the instance is hosted on and may be different on each instance.

Postgres, if configured correctly and given the resources can store almost an unlimited amount of data but should not be used as a dumping ground for storage.

> Learning all the features of PostgreSQL will help you manage your databases more efficiently.

## The core team
The members of the PostgreSQL Global Developer Group (PGDG) are the core members that are responsible for the development of Postgres.

They work hard and deliver a single production release every year and then work towards maintaining it and removing any bugs and errors that might come after the release as well as develop the next version of Postgres.

## ACID compliant
PostgreSQL is fully ACID compliant, meaning that it supports atomicity, consistency, isolation, and durability.

- Atomicitiy means that each command is processed as a single instruction not matter how complex it might be.
- Consistency means that the data stored in the database will be consistent throughout operations and if a operation fails the data won't be changed.
- Isolation means that the database is able to handle concurrent operations without damaging or changing the data.
- Durability means that Postgres tries to protect the data as much as it can in case of a hardware or software failure.

## Extensions
Postgres comes with it's own version of SQL called PgSQL that allows developers and database admins to create functions, procedures, triggers, and views according to their needs.

Postgres can also be extended with embedded languages such as Perl and Bash and extensions like GIS that allow it to handle geo spatial data.