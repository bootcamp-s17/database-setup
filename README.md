# Database Setup

You'll need a local installation of PostgreSQL to host your databases, and a GUI to more easily view your data.

## PostgreSQL

https://www.postgresql.org/

The installation instructions are terrible - you've been warned.

You download the binary for your OS and run it. The setup program will walk you through installation.

You'll be asked to set up a master username/password. Remember these! You will need them later when we set up databases for our projects.

Also, accept the default port of 5432. 

## GUI database management tool

### PSequel for MacOS

http://www.psequel.com/

### PGAdmin for everyone

https://www.pgadmin.org/

## Put it all together

Start the PostgreSQL server. (Instructions vary by OS.)

Open psql. (On my Mac, this is an option when PostgreSQL is started.)

Create a new user, and then a new database owned by that user:

  Janine=# CREATE USER exampledb_user WITH PASSWORD 'example'; 
  Janine=# CREATE DATABASE exampledb_dev OWNER exampledb_user;

You can close psql now.

Open your GUI.

Create a connection for the database you just created.

If you can view the database (it will be empty), you're done!


