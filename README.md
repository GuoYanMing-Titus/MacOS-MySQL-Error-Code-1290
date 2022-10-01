# MacOS-MySQL-Error-Code-1290 
Error Code: 1290. The MySQL server is running with the --secure-file-priv option so
1. edit my.cnf
~~~ shell
sudo vim /etc/my.cnf
~~~

2. insert to my.cnf
~~~
[mysqld]
secure_file_priv = ''
local_infile = "ON"
~~~

3. Restart MySQL server.


# OS errno 13 - Permision denied
Error Code: 1. Can't create/write to file '/Users/forsql/customers2.csv' (OS errno 13 - Permission denied)

1. make a folder for MySQL
~~~
sudo mkdir /Users/forsql
sudo chown mysql /Users/forsql
~~~
