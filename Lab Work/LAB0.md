# Lab 1

## Database Language

- DDL (Data Definition Language)
- DML (Data Manipulation Langugage)

## Initial Steps

1. Start Apache and MySql in XAMPP
2. Open PhpMyAdmin

## RDBMS

- Data are managed as Tables.

## TABLES

- We need no. of coloumns
- Rows will increase dynamically
- We can have multiple tables in 1 database
- one project mostly requires only one database

- Truncate: It deletes the data but preserves the Table Structure.
- Drop: It deletes the table and data.

## DDL

- CREATE
- ALTER

## DML

- INSERT
- UPDATE
- DELETE
- SELECT

## Schema and Instance
- Schema is the col name
- Instance is the values in that col
## LETS CREATE A DATABASE AND TABLE USING CREATE

- lets Create a database

```sql
CREATE DATABASE db.name
```

- Now lets create a table

```sql
CREATE TABLE table.name
```

- The aboce code doesn't work as we need to specify the coloum names and data type

```sql
CREATE TABLE Student(
    roll int,
    name text,
    address text,
    phone int
)
```

- Now we have supplied the required coloums the table is now created.

## ADDING DATA TO THE TABLE

- We use DML command Insert to do this
- We need to maintain the order of insertion

```sql
INSERT INTO TableName(col1,col2) VALUES (val1,val2)
```

- we can also use the syntax below

```sql
INSERT INTO TableName VALUES (val1, val2)
```

- using the above sql command can cause future problems which we will see in future lab

## Retrieving Information from Table

- We use the SELECT command to retrieve the information.

```sql
SELECT * FROM TableName
```

- The above code will fetch all data from the table

- To fetch Particular coloumns from a table we specify the coloumn name

```sql
SELECT col1 FROM student
```

## Truncate and Drop

```sql
TRUNCATE TABLE tableName
```

- The above code deletes the data from table

```sql
DROP TABLE TableName
```

- The above code delets the table entirely

- To delete Database we use

```sql
DROP DATABASE DatabaseName
```

# Question

1. Create database CMS
2. Create tables staff (sid, name, designation,salary) and department (did,name,block)
3. Insert one record for Each File
4. Truncate and Drop Tables
5. Drop DataBase
