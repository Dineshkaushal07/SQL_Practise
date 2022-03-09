#Creating a Database 
```
CREATE DATABASE database_name;
```
#Using a Database 
```
USE database_name;
```
#List all the tables in the database
```
SHOW TABLES
```
#List tables on specific names
<!--  After like we use wildcard operators so please read them to use them. -->
```
SHOW TABLES LIKE '%string-to-be-matched%' 
```
#Comments in SQL
```
-- For Single Line comment
/* */ for multiline comments
```
#Create a new TABLE
```
CREATE TABLE IF NOT EXISTS Table_name(
      Column1 datatype,
      Column2 datatype
      ...
      );
E.g. - CREATE TABLE IF NOT EXISTS students (
  id INTEGER ,
  name varchar ,
  gender varchar 
);
```
#Insert records in a Table
```
INSERT INTO Table_name VALUES (Value1,Value2)
E.g. - INSERT INTO students VALUES (1, 'Ryan', 'M');
```
#Fetching records
```
SELECT * FROM Table_name
```
#Fetching records with a Condition
```
SELECT * FROM Table_name WHERE Column_name=particularvalues
```
#Group By Clause 
It is used when we need to group the columns, here same values has same group, we search for distinct combination of values of columns on which we have grouped.
its mainly used when we have to use aggregate Functions.
```
SELECT sum(ID) from students group by ID

#Complete Example 
```
CREATE TABLE students (
  id INTEGER ,
  name TEXT  ,
  gender TEXT 
);
-- insert some values
INSERT INTO students VALUES (1, 'Ryan', 'M');
INSERT INTO students VALUES (2, 'Joanna', 'F');

-- fetch some values
SELECT * FROM students WHERE gender = 'F';
```
