# chapter1_1
create table kakeibo(
 hiduke   date,
 himokuid integer,
 memo     varchar(100),
 nyukin   integer,
 syukkin  integer
);



mysql> -- 1行のコメント
mysql> -- 　1行のコメント
mysql> ^C
mysql> --　１行のコメント
    ->
    ->
    -> ^C
mysql> --　１行のコメント
    -> ^C
    -> ^C
mysql> /*複数行の
   /*> コメント*/
mysql> #１行のコメント
mysql> #１行のコメント
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sakila             |
| sys                |
| world              |
+--------------------+
6 rows in set (0.11 sec)

mysql> SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sakila             |
| sys                |
| world              |
+--------------------+
6 rows in set (0.00 sec)

mysql> create database 12java;
Query OK, 1 row affected (0.24 sec)

mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| 12java             |
| information_schema |
| mysql              |
| performance_schema |
| sakila             |
| sys                |
| world              |
+--------------------+
7 rows in set (0.05 sec)

mysql> use 12java;
Database changed
mysql> create table kakeibo(
    ->  hiduke   date,
    ->  himokuid integer,
    ->  memo     varchar(100),
    ->  nyukin   integer,
    ->  syukkin  integer
    -> );
Query OK, 0 rows affected (1.78 sec)

mysql> show columns from kakeibo;
+----------+--------------+------+-----+---------+-------+
| Field    | Type         | Null | Key | Default | Extra |
+----------+--------------+------+-----+---------+-------+
| hiduke   | date         | YES  |     | NULL    |       |
| himokuid | int          | YES  |     | NULL    |       |
| memo     | varchar(100) | YES  |     | NULL    |       |
| nyukin   | int          | YES  |     | NULL    |       |
| syukkin  | int          | YES  |     | NULL    |       |
+----------+--------------+------+-----+---------+-------+
5 rows in set (0.12 sec)

mysql> alter table kakeibo rename column himokuid to himoku_id;
Query OK, 0 rows affected (0.29 sec)
Records: 0  Duplicates: 0  Warnings: 0

mysql> show columns from kakeibo;
+-----------+--------------+------+-----+---------+-------+
| Field     | Type         | Null | Key | Default | Extra |
+-----------+--------------+------+-----+---------+-------+
| hiduke    | date         | YES  |     | NULL    |       |
| himoku_id | int          | YES  |     | NULL    |       |
| memo      | varchar(100) | YES  |     | NULL    |       |
| nyukin    | int          | YES  |     | NULL    |       |
| syukkin   | int          | YES  |     | NULL    |       |
+-----------+--------------+------+-----+---------+-------+
5 rows in set (0.05 sec)

mysql> alter table kakeibo modify himoku_id varchar(1);
Query OK, 0 rows affected (4.45 sec)
Records: 0  Duplicates: 0  Warnings: 0

mysql> show columns from kakeibo;
+-----------+--------------+------+-----+---------+-------+
| Field     | Type         | Null | Key | Default | Extra |
+-----------+--------------+------+-----+---------+-------+
| hiduke    | date         | YES  |     | NULL    |       |
| himoku_id | varchar(1)   | YES  |     | NULL    |       |
| memo      | varchar(100) | YES  |     | NULL    |       |
| nyukin    | int          | YES  |     | NULL    |       |
| syukkin   | int          | YES  |     | NULL    |       |
+-----------+--------------+------+-----+---------+-------+
5 rows in set (0.05 sec)

mysql> alter table kakeibo add id ingt;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'ingt' at line 1
mysql> alter table kakeibo add id int;
Query OK, 0 rows affected (0.39 sec)
Records: 0  Duplicates: 0  Warnings: 0

mysql> alter table kakeibo modify id int after nyukin;
Query OK, 0 rows affected (2.23 sec)
Records: 0  Duplicates: 0  Warnings: 0

mysql> show columns from kakeibo;
+-----------+--------------+------+-----+---------+-------+
| Field     | Type         | Null | Key | Default | Extra |
+-----------+--------------+------+-----+---------+-------+
| hiduke    | date         | YES  |     | NULL    |       |
| himoku_id | varchar(1)   | YES  |     | NULL    |       |
| memo      | varchar(100) | YES  |     | NULL    |       |
| nyukin    | int          | YES  |     | NULL    |       |
| id        | int          | YES  |     | NULL    |       |
| syukkin   | int          | YES  |     | NULL    |       |
+-----------+--------------+------+-----+---------+-------+
6 rows in set (0.05 sec)

mysql> alter table kakeibo modify id int first;
Query OK, 0 rows affected (1.53 sec)
Records: 0  Duplicates: 0  Warnings: 0

mysql> show columns from kakeibo;
+-----------+--------------+------+-----+---------+-------+
| Field     | Type         | Null | Key | Default | Extra |
+-----------+--------------+------+-----+---------+-------+
| id        | int          | YES  |     | NULL    |       |
| hiduke    | date         | YES  |     | NULL    |       |
| himoku_id | varchar(1)   | YES  |     | NULL    |       |
| memo      | varchar(100) | YES  |     | NULL    |       |
| nyukin    | int          | YES  |     | NULL    |       |
| syukkin   | int          | YES  |     | NULL    |       |
+-----------+--------------+------+-----+---------+-------+
6 rows in set (0.04 sec)

mysql> alter table kakeibo drop id;
Query OK, 0 rows affected (2.52 sec)
Records: 0  Duplicates: 0  Warnings: 0

mysql> show columns from kakeibo;
+-----------+--------------+------+-----+---------+-------+
| Field     | Type         | Null | Key | Default | Extra |
+-----------+--------------+------+-----+---------+-------+
| hiduke    | date         | YES  |     | NULL    |       |
| himoku_id | varchar(1)   | YES  |     | NULL    |       |
| memo      | varchar(100) | YES  |     | NULL    |       |
| nyukin    | int          | YES  |     | NULL    |       |
| syukkin   | int          | YES  |     | NULL    |       |
+-----------+--------------+------+-----+---------+-------+
5 rows in set (0.01 sec)

mysql> alter table kakeibo rename housekeeping_book;
Query OK, 0 rows affected (0.44 sec)

mysql> show tables;
+-------------------+
| Tables_in_12java  |
+-------------------+
| housekeeping_book |
+-------------------+
1 row in set (0.15 sec)

mysql> drop table housekeeping_book;
Query OK, 0 rows affected (0.38 sec)

mysql> show tables;
Empty set (0.03 sec)
