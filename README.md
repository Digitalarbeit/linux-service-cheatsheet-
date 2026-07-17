# OLLAMA

## Stop immediately
```bash
sudo systemctl stop ollama
```

## Disable autostart on boot (stays off after reboot)
```bash
sudo systemctl disable ollama
```

## Start manually when needed
```bash
sudo systemctl start ollama
```

## Re-enable autostart on boot
```bash
sudo systemctl enable ollama
```

## Check status
```bash
systemctl status ollama
```
```bash
systemctl is-enabled ollama
```
```bash
systemctl is-active ollama
```

## Update Ollama
```bash
curl https://ollama.ai/install.sh | sh
```

## List all Ollama models
```bash
ollama list
```

## Download & run models
```bash
ollama pull model
ollama run model
```

## Delete models
#### Delete model (frees up disk space)
```bash
ollama rm model
```
#### Unload model from RAM (does not delete it)
```bash
ollama stop model
```

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

## Access PostgreSQL as the postgres user
### Step 1: Switch to the postgres system user
```bash
sudo su postgres
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
