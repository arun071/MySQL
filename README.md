
# MySQL Commands
## DataBase
#### To Create a Database
``` 
CREATE DATABASE dbName; 
``` 

#### To Drop a Database
```
DROP DATABASE dbName;
```
## Table
#### To Create a Table
```
CREATE TABLE tableName (
    column1 datatype,
    column2 datatype,
    ...
);
``` 

#### To Drop a Table
```
DROP TABLE tableName;
```

#### To Insert Data into a Table
```
INSERT INTO tableName (column1, column2, ...)
VALUES (value1, value2, ...);
``` 

#### To Update Data in a Table
```
UPDATE tableName
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

#### To Delete Data from a Table
```
DELETE FROM tableName
WHERE condition;
``` 

#### To Select Data from a Table

```
SELECT column1, column2, ...
FROM tableName
WHERE condition;
``` 

#### To Add a Column to a Table
```
ALTER TABLE tableName
ADD columnName datatype;
``` 

#### To Drop a Column from a Table
```
ALTER TABLE tableName
DROP COLUMN columnName;
```

## SELECT
#### To select a column from a database table
``` 
SELECT column1, column2, ...
FROM table;
``` 
#### To select all columns from a database table
``` 
SELECT *
FROM tableName;
``` 

#### SQL SELECT WHERE Clause
```
SELECT *
FROM tableName
WHERE condition;

```

## SQL Operators
### The WHERE clause uses operators to construct conditions. Some of the commonly used operators are:

#### 1. Equal to Operator (=)
``` 
-- select all columns from Customers table with first name 'John'
SELECT *
FROM Customers
WHERE first_name = 'John';
``` 
#### 2. Greater than (>)
``` 
-- select all columns from Customers table with age greater than 25
SELECT *
FROM Customers
WHERE age > 25;
``` 

#### 3. AND Operator (AND)

```
-- select all columns from Customers table with last_name 'Doe' and country 'USA'
SELECT *
FROM Customers
WHERE last_name = 'Doe' AND country = 'USA';

```

#### 4 .SQL OR Operator
``` 
-- select first and last name of customers
-- who either live in the USA
-- or have the last name 'Doe'

SELECT first_name, last_name
FROM Customers
WHERE country = 'USA' OR last_name = 'Doe';
``` 
#### 5 .SQL NOT Operator
``` 
-- select customers who don't live in the USA

SELECT first_name, last_name
FROM Customers
WHERE NOT country = 'USA';
``` 

#### Combining Multiple Operators

```
-- select customers who live in either USA or UK and whose age is less than 26

SELECT *
FROM Customers
WHERE (country = 'USA' OR country = 'UK') AND age < 26;

```

#### To Create an Index
```
CREATE INDEX indexName
ON tableName (columnName);
``` 

#### To Drop an Index
``` 
DROP INDEX indexName
ON tableName;
```

#### To Create a View
``` 
CREATE VIEW viewName AS
SELECT column1, column2, ...
FROM tableName
WHERE condition;
``` 

#### To Drop a View
```
DROP VIEW viewName;
``` 

#### To Grant Privileges
```
GRANT ALL PRIVILEGES ON dbName.*
TO 'username'@'host'
IDENTIFIED BY 'password';
```

#### To Revoke Privileges
```
REVOKE ALL PRIVILEGES ON dbName.*
FROM 'username'@'host';
``` 





