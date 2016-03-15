# mysql

## create

```
>
create table posts
(
  id serial primary key,
  title varchar(255) not null,
  body text, sort_id int,
  created timestamp default CURRENT_TIMESTAMP
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
create table users (
    id integer primary key autoincrement,
    name text not null,
    email text unique,
    age integer default 20
);
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
