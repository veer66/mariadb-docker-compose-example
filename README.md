# mariadb-docker-compose-example

I want: 

* My database to use UTF-8
* A database to be created by docker-compose

I'm afraid that I'm going to forget or lose this example with my SSD, so I posted this on the Internet. I'm glad if it is useful for you too.

## Run

````
sudo docker-compose up
````

## Connect

````
$ mysql -umyusr -pmyusrpass mydb --protocol=tcp
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 10
Server version: 10.3.7-MariaDB-1:10.3.7+maria~jessie mariadb.org binary distribution

Copyright (c) 2000, 2017, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [mydb]> status
--------------
mysql  Ver 15.1 Distrib 10.1.29-MariaDB, for debian-linux-gnu (x86_64) using readline 5.2

Connection id:		10
Current database:	mydb
Current user:		myusr@127.0.0.1
SSL:			Not in use
Current pager:		stdout
Using outfile:		''
Using delimiter:	;
Server:			MariaDB
Server version:		10.3.7-MariaDB-1:10.3.7+maria~jessie mariadb.org binary distribution
Protocol version:	10
Connection:		localhost via TCP/IP
Server characterset:	utf8
Db     characterset:	utf8
Client characterset:	utf8
Conn.  characterset:	utf8
TCP port:		3306
Uptime:			7 min 53 sec

Threads: 7  Questions: 8  Slow queries: 0  Opens: 17  Flush tables: 1  Open tables: 11  Queries per second avg: 0.016
--------------

MariaDB [mydb]>
````
