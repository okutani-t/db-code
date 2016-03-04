# mysql

## start stop auto-start

```
$ service mysqld start
$ service mysqld stop
```

## login

```
$ mysql -u root -p
$ mysql -u dbuser -p piyo_db
```

## root pass setting

```
set password for root@localhost=password('hoge');
```

## create database

```
> create database piyo_db;
```

## setting db_user

```
> grant all on piyo_db.* to dbuser@localhost identified by 'password';
```

## show

```
> show databases;
> show tables;
```

---

## drop

```
> drop database piyo_db;
```

## chenge table

```
> use moge_db;
```

## exit

```
> exit
```

# postgresql

## start stop

```
$ service postgresql start
$ service postgresql stop
$ chkconfig postgresql on
```

## show users

```
$ id postgres
```

## create database

```
$ createdb piyo_db
```

## login

```
$ psql piyo_db
```

## show

```
$ psql -l
> \l
```

## drop

```
$ dropdb piyo_db
```

## exit

```
> \q
```

---

# sqlite

## start

```
$ sqlite3 piyo.sqlite3
```

## exit

```
> .exit
```
