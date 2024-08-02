# History of PostgreSQL
In 1986, Professor Michael Stonebreaker started the post-ingres project after creating ingres which was the predecessor of Postgres in hopes to change the database landscape of the time and create a database engine that could be extended by the users using objects.

Version 4.2 of Postgres was first released in 1994 under an MIT license that allowed other people to collaborate in this project as well. Postgres used QUEL as it's main programming language at the time which was then replaced with SQL.

In 1996 the project gained enough traction and funding to host a server and started working on the re-branded PostgreSQL project which has been under development for over 30 years now.

## Database users
PostgreSQL runs as a service/daemon on the server or computer that it's installed on and then server is known as a cluster since it can host multiple databases.

Each database is stored in an isolated space and a user can only access a single database at a time. Users are defined cluster-wide and are not tied to a single database and can connect to as many databases as they are allowed to.

Normal users are users that are allowed to run a specific set of commands on the databases they are allowed to access. Superusers can do anything they desire with the database.

PostgreSQL stores it's internal and user data into the server's local storage in the form of catalogs that are special tables that show the specification of the instance depending on the user accessing them.

## Internal File system
In order to make the data persistent, PostgreSQL relies on the file system of the server it is hosted on and therefore the file system of the instance plays an important part in the performance of your PostgreSQL instance.

All of the internal and user data is stored in a file system directory called `PGDATA`. This directory represents the contents that the cluster is showing as databases. A single instance of PostgreSQL can access different `PGDATA` directories and therefore contain different databases in it.

> The `PGDATA` directory and it's sub-directories need to be initialized before they can be used.

The `PGDATA` directory is where PostgreSQL looks for its configuration and data files and also contains the `Write-Ahead-Logs` and the data storage as well.

> Without the WALs and data storage the cluster can not guarantee the consistency of the data or sometimes even start at all.

## Write Ahead Logs
Write Ahead Logs or `WALs` for short are a technology that many database systems use for their internal logging. The main concept of a `WAL` is that before confirming any operation it writes the intent as a log.

In case the cluster crashes, the database already knows what operations were completed and what data needs to be recovered when it reads the `WALs`.

## Postmaster
When the cluster is started, a single process known as the _postmaster_ is launched that bootstraps the entire instance and starts the needed processes needed to manage the database and wait for any incoming connections.

If a user connection is made over TCP/IP then the postmaster needs to fork a process called the _backend_ process that is responsible for making sure that a single user connects to the database.

> A backend process is launched for each individual connected user.

## Understanding the cluster
PostgreSQL is an enterprise level database management solution and by no means it is a simple software. But, due to the great design, implementation, and documentation created for it learning the inner workings of PostgreSQL isn't as complicated as it might seem.

There are two main ways to interact with your cluster, using the command line client `PSQL` that comes with the PostgreSQL installer and is the default method of connecting to the cluster. The second one is to use a GUI-based client such as `PgAdmin`.

> Managing a cluster means being able start, stop, take control, and get information about the status of a PostgreSQL instance.

## Command line
`Pg_ctl` is a command line utility that gets installed on your system alongside PostgreSQL and is used to manage the cluster. 

Some of the common commands are:

| Command                  | Description                                                                                                                                   |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- |
| Start, stop, and restart | Start, stops, or restarts the cluster.                                                                                                        |
| Status                   | displays the current status of the cluster.                                                                                                   |
| Init                     | Initializes a new cluster or re-initializes an already existing one. Re-initializing a cluster removes all of the previous data stored in it. |
| Reload                   | Reloads the server when there's a config change.                                                                                              |
| Promote                  | Changes a replica server to a standby one.                                                                                                    |

> Pg_ctl works with the postmaster by giving it commands that further gives commands to other services and processes. 

Pg_ctl also needs to know about the `PGDATA` directory. You can set the location of it by defining a environment variable or using the -D flag on the command line.

## Server Processes
The `POSTMASTER` process is the first process that is launched when the cluster is started that is responsible for starting and managing other processes.

| Process                      | Description                                                              |
| ---------------------------- | ------------------------------------------------------------------------ |
| Checkpoint                   | Responsible for executing checkpoints that maintain the persistent data. |
| background writer            | Stores data into permanent storage from memory                           |
| walwriter                    | Writes WALs                                                              |
| logical replication launcher | Handles logical replication                                              |

> Processes are based on the configurations of the server, and so each server can have different processes running.




