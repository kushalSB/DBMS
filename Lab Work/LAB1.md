# Title: Data Definiton Language (DDL) Commands

# Objective: To practise and implement data definition language commands and constraints

# Procedure

1. DDL Command

   - is used to communicate with database.
   - is used to
     - Create an Object
     - Alter Structure of object
     - to drop The object created.
   - Commands used are: CREATE, ALTER, DROP, TRUNCATE

2. Constraints

   - Constraints are rules or definition that govern the operations in the data. Constraints can be done at coloumn level or at the table level depending upon the requirement.

   Three types of Constraints.

   1. Integrity Constraints
      - NOT NULL Constraint
      - NULL Constraint
      - UNIQUE Constraints
   2. Entity Constraint (Primary Key)
   3. Refrential Constraint (Foreign Key)

# Constriant Code

1. NOT NULL

Enforce field to always have a value.

```sql
CREATE TABLE teacher
(
    T_id int NOT NULL,
    T_NAME varchar(50) NOT NULL
)
```

# Adding Constraints

1. Adding Constraints

- First Alter Table

```sql
ALTER TABLE tablename
ADD CONSTRAINT constraint_name (filedname,fieldname,...)
```

We can add Primary key, Foreign Key, Unique, Not Null and Check as constraints.

2. To add Foreign Key

```sql
ALTER TABLE tablename
ADD CONSTRAINT fk_name FOREIGN KEY  (field_name) REFERENCE table_name(filed_name)
```

3. To add Primary Key

```sql
ALTER TABLE tablename
ADD CONSTRAINT pk_name PRIMARY KEY (filedname,fieldname,...)
```

- Just Replace PRIMARY KEY with UNIQUE, to ensure every record in that field is unique
- PRIMARY KEY id UNIQUE and NOT NULL

# Removing Constraints

use the syntax below

```sql
ALTER TABLE tablename
DROP CONSTRAINT constraint_name
```

- it is necessary to remove constraints of Fields that are foreign key if we want to drop that field or table.
