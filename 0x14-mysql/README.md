# 0x14. MySQL

## Task
### 0. Install MySQL
* MySQL distribution must be 5.7.x

### 1. Let us in!
* Create a MySQL user named holberton_user on both web-01 and web-02 with the host name set to localhost and the password projectcorrection280hbtn. This will allow us to access the replication status on both servers.
* Make sure that holberton_user has permission to check the primary/replica status of your databases.

### 2. If only you could see what I've seen with your eyes
* Createe a database named tyrell_corp
* Within the tyrell_corp database create a table named nexus6 and add at least one entry to it.
* Make sure that holberton_user has SELECT permissions on your table so that we can check that the table exists and is not empty.

### 3. Quite an experience to live in fear, isn't it?
* The name of the new user should be replica_user, with the host name set to %, and can have whatever password you’d like.
* replica_user must have the appropriate permissions to replicate your primary MySQL server.
* holberton_user will need SELECT privileges on the mysql.user table in order to check that replica_user was created with the correct permissions.

### 4. Setup a Primary-Replica infrastructure using MySQL
* Redundancy: If you lose one of the database servers, you will still have another working one and a copy of your data
* Load distribution: You can split the read operations between the 2 servers, reducing the load on the primary member and improving query response speed

### 5. MySQL backup
* The MySQL dump must contain all your MySQL databases
* The MySQL dump must be named backup.sql
* The MySQL dump file has to be compressed to a tar.gz archive
* This archive must have the following name format: day-month-year.tar.gz
* The user to connect to the MySQL database must be root
* The Bash script accepts one argument that is the password used to connect to the MySQL database
