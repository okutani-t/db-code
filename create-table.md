# mysql

## create

```
>
create table users (
    id int not null auto_increment primary key,
    name varchar(255),
    email varchar(255) unique,
    password char(32),
    sex enum('male', 'female'),
    memo text default 'sample memo',
    created datetime
);
```

## show

```
> desc users;
> select * from users;
> select * from users \\G;
```

## drop

```
> drop table users;
```

---

# postgresql

## create

```
>
create table posts (
    id serial primary key,
    title varchar(255) not null,
    body text check(length(body) > 5),
    is_draft boolean default TRUE,
    created timestamp default 'now'
);
```

## show

```
> \dt
> select * from posts;
```

## rename

```
> alter table posts rename to myposts;
```

## drop

```
> drop table posts;
```

---

# sqlite

## create

```
>

```

## show

```
> .tables
> .schema
> select * from users;
```

## rename

```
> alter table users rename to myusers;
```

## drop

```
> drop table users
```
