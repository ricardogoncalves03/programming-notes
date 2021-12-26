<div align="center"> <h1>PSQL documentation</h1> </div>  


![psql](resources/postgresql.svg)

## 1 - Check psql status and connect

---
### PSQL status
```bash
sudo systemctl status postgresql
```
### Connect to the database as the superuser
```bash
sudo -u postgres psql  
```

## 2 - User

---
### List Users 
```bash
\du  
```
### Create User with permission to create databases
```bash
CREATE USER user1 WITH PASSWORD 'password' CREATEDB;
```

## 3 - Databases

---
### List Databases
```bash
\l
```
### Create new Database
```bash
CREATE DATABASE yourdbname;
```
### Grant privileges
```bash
GRANT ALL PRIVILEGES ON DATABASE yourdbname TO youruser;
```
### Connect to database
```bash
\c database_name
```
### Show tables
```bash
\dt
```
### Connect to database as a specific user
```bash
\c database_name user_name localhost
```

