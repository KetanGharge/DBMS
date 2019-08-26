# DBMS


Enter password: ****
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 3
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
40 rows in set (0.00 sec)

mysql> CREATE DATABASE Gohan;
Query OK, 1 row affected (0.02 sec)

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
41 rows in set (0.00 sec)

mysql> USE Gohan;
Database changed
mysql> CREATE table ProductCategory
    -> (
    -> ProductCategoryID int,Name varchar(20)
    -> );
Query OK, 0 rows affected (0.06 sec)

mysql> INSERT INTO ProductCategory VALUES(1,'BIKES');
Query OK, 1 row affected (0.05 sec)

mysql> INSERT INTO ProductCategory VALUES(2,'Accessories');
Query OK, 1 row affected (0.02 sec)

mysql> INSERT INTO ProductCategory VALUES(3,'Clothing');
Query OK, 1 row affected (0.05 sec)

mysql> INSERT INTO ProductCategory VALUES(4,'Components');
Query OK, 1 row affected (0.03 sec)

mysql> INSERT INTO ProductCategory VALUES(5,'Misc');
Query OK, 1 row affected (0.03 sec)

mysql> SELECT *FROM ProductCategory;
+-------------------+-------------+
| ProductCategoryID | Name        |
+-------------------+-------------+
|                 1 | BIKES       |
|                 2 | Accessories |
|                 3 | Clothing    |
|                 4 | Components  |
|                 5 | Misc        |
+-------------------+-------------+
5 rows in set (0.00 sec)

mysql> UPDATE ProductCategory
    -> SET Name='Miscellaneous'
    -> WHERE ProductCategoryID='5';
Query OK, 1 row affected (0.03 sec)
Rows matched: 1  Changed: 1  Warnings: 0

mysql> SELECT *FROM ProductCategory;
+-------------------+---------------+
| ProductCategoryID | Name          |
+-------------------+---------------+
|                 1 | BIKES         |
|                 2 | Accessories   |
|                 3 | Clothing      |
|                 4 | Components    |
|                 5 | Miscellaneous |
+-------------------+---------------+
5 rows in set (0.00 sec)

mysql> DELETE FROM ProductCategory
    -> WHERE ProductCategoryID='5';
Query OK, 1 row affected (0.03 sec)

mysql> SELECT *FROM ProductCategory;
+-------------------+-------------+
| ProductCategoryID | Name        |
+-------------------+-------------+
|                 1 | BIKES       |
|                 2 | Accessories |
|                 3 | Clothing    |
|                 4 | Components  |
+-------------------+-------------+
4 rows in set (0.00 sec)

mysql> TRUNCATE TABLE ProductCategory;
Query OK, 0 rows affected (0.02 sec)

mysql> SELECT *FROM ProductCategory;
Empty set (0.00 sec)

mysql> DROP TABLE ProductCategory;
Query OK, 0 rows affected (0.05 sec)

mysql> SELECT *FROM ProductCategory;
ERROR 1146 (42S02): Table 'gohan.productcategory' doesn't exist
mysql>
