# MacOS-MySQL-Error-Code-1290 and OS errno 13 - Permision denied
Error Code: 1290. The MySQL server is running with the --secure-file-priv option so

1. make a folder for MySQL
~~~
sudo mkdir /Users/forsql
sudo chown mysql /Users/forsql
~~~

2. edit my.cnf
~~~ shell
sudo vim /etc/my.cnf
~~~

3. insert to my.cnf
~~~
[mysqld]
secure_file_priv = ''
local_infile = "ON"
~~~

4. Restart MySQL server.

