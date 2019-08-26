Enter password: ****
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 4
Server version: 5.1.38-community MySQL Community Server (GPL)

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| Gita               |
| adventureworks     |
| aniket             |
| assignment         |
| assignments        |
| day                |
| dee                |
| etour              |
| exam               |
| feedback           |
| fleet              |
| function           |
| gohan              |
| goku               |
| location           |
| login              |
| mydata             |
| mydb               |
| mydemodata         |
| myproject          |
| mysql              |
| mysql1             |
| office             |
| parth              |
| ph                 |
| phadkar            |
| php                |
| pps                |
| pract              |
| practice           |
| project            |
| projectdemo        |
| sam                |
| sd                 |
| studnt             |
| test               |
| testdb             |
| tuzadb             |
| user               |
| vita               |
+--------------------+
41 rows in set (0.09 sec)

mysql> CREATE DATABASE Vegeta;
Query OK, 1 row affected (0.00 sec)

mysql> SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| Gita               |
| adventureworks     |
| aniket             |
| assignment         |
| assignments        |
| day                |
| dee                |
| etour              |
| exam               |
| feedback           |
| fleet              |
| function           |
| gohan              |
| goku               |
| location           |
| login              |
| mydata             |
| mydb               |
| mydemodata         |
| myproject          |
| mysql              |
| mysql1             |
| office             |
| parth              |
| ph                 |
| phadkar            |
| php                |
| pps                |
| pract              |
| practice           |
| project            |
| projectdemo        |
| sam                |
| sd                 |
| studnt             |
| test               |
| testdb             |
| tuzadb             |
| user               |
| vegeta             |
| vita               |
+--------------------+
42 rows in set (0.00 sec)

mysql> USE Vegeta;
Database changed
mysql> CREATE TABLE Test(ID int NOT NULL,Name varchar(20),Pin int,PRIMARY KEY(ID));
Query OK, 0 rows affected (0.06 sec)

mysql> INSERT INTO Test VALUES(101,'ABC',401);
Query OK, 1 row affected (0.03 sec)

mysql> INSERT INTO Test VALUES(102,'DEF',501);
Query OK, 1 row affected (0.03 sec)

mysql> INSERT INTO Test VALUES(102,'GHI',601);
ERROR 1062 (23000): Duplicate entry '102' for key 'PRIMARY'
mysql> INSERT INTO Test VALUES(103,'GHI',601);
Query OK, 1 row affected (0.03 sec)

mysql> SELECT *from Test;
+-----+------+------+
| ID  | Name | Pin  |
+-----+------+------+
| 101 | ABC  |  401 |
| 102 | DEF  |  501 |
| 103 | GHI  |  601 |
+-----+------+------+
3 rows in set (0.00 sec)

