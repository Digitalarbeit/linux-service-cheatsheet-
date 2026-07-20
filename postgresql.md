# POSTGRESQL

## Stop immediately
```bash
sudo systemctl stop postgresql
```

## Disable autostart on boot
```bash
sudo systemctl disable postgresql
```

## Start manually when needed
```bash
sudo systemctl start postgresql
```

## Re-enable autostart
```bash
sudo systemctl enable postgresql
```

## Check status
```bash
systemctl status postgresql
```
```bash
systemctl is-enabled postgresql
```
```bash
systemctl is-active postgresql
```

## change password in sql shell
```bash
sudo systemctl enable postgresql
```

## Access PostgreSQL as the postgres user
### Step 1: Switch to the postgres system user
```bash
sudo -u postgres psql
ALTER USER postgres WITH PASSWORD 'your_new_password';
```

### Step 2: Enter the PostgreSQL interactive shell
```bash
psql
```

### Check available database
```bash
\l
```

### create new database
```bash
create database your_db_name;
```

### connect to database
```bash
\c databse_name
```

### delete database
```bash
drop database database_name;
```

### create tables in database (example)
```bash
create table tablename (id serial primary key, name text, address text, age int);
```

### check existing tables in database
```bash
\d
```

### insert data into table (example) - Single quotes for values
```bash
insert into tablename (name, address, age) values ('Digitalarbeit', 'Germany - Italy', 42);
```

### reading from tables
```bash
select * from tablename;
```

### condition select
```bash
select * from tablename where condition;
```
```bash
select * from tablename where name='John';
```

### update table
```bash
update tablename set value_to_set where reference_table;
```
```bash
update tablename set age=18 where id=1;
```

### delete entry
```bash
delete from tablename where condition;
```
```bash
delete from tablename where id=1;
```

