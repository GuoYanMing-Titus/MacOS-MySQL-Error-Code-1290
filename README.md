# MacOS-MySQL-Error-Code-1290 and OS errno 13 - Permision denied
Error Code: 1290. The MySQL server is running with the --secure-file-priv option so it cannot execute this statement
# deep-pitcher
Estimates pitch of human vocal from songs by vocal separation with machine learning

1. 
~~~ shell
sudo vim /etc/my.cnf
~~~
~~~ sql
CREATE USER 'itdb' IDENTIFIED BY 'itdb';
GRANT ALL PRIVILEGES ON itdb.* TO 'itdb' WITH GRANT OPTION;
GRANT FILE on *.* to itdb;
FLUSH PRIVILEGES;
~~~

Error Code: 1. Can't create/write to file '/Users/forsql/customers2.csv' (OS errno 13 - Permission denied)
