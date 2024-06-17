
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





