# Database
It is an Organized collection of information (or) data. it can be accessed by multiple people simultaneously. it also stores massive amounts of data, it can perform complex tasks while accessing data using databases allow us to store large amounts of data while keeping it quick and easy to access.

## Relational database

A Structured database containing tables that are related to each other.

### Key: 

The columns in a RDB that relate two tables to each other are called keys. They are two types of keys.

  - Primary Key
  - Foreign key

**Primary Key** : A column where every row has a unique entry. it should not have any duplicate (or) null (or) empty values. it allows us to uniquely identify every row in a table.

**Foreign key** : A column in a table that is a primary key in another table. unlike primary, foreign keys can have empty & Duplicate values. They allows us to connect two tables together.

NOTE: A table can only have one primary key, but multiple foreign keys.

## Structured query language (SQL) :

A Programming language used to create, interact with, and request information from a database. In terms of structure, SQL provides results that are more easily readable and that can be adjusted more quickly then when using Linux.

**Query** : A Request for data from a database table or a combination of tables.

**Log** : A Record of events that occur within organization systems. SQL uses the structured query language (SQL), it is a standardized language with specific keyworks and clauses for filtering data across different SQL databases.

EX: SQL keywords and clauses are WHERE, SELECT, JOIN.

### Joining Tables : 

Some security related descisions require information from different tables. SQL allows the analyst to join multiple tables together when returning data. it doesnt allow data to be connected to other information on your computer.

## Test Case 
if want to get employee-id & Device-id from an employees tables. Now we need to write a query to only get two columns. The two most common queries are

      |__Employees___|
      |  Employee_id |
      |  device_id   |
      |  User name   |
      |  Department  |
      |___Office_____|

The Most common queries are
     
  - SELECT ---> Indicates which columns to returns
  - FROM ---> Indicates which table to query

        EX: SELECT employee-id, device-id
            FROM employees;
    
  - ORDER BY ---> It is an imp keyword for organizing the data that we extract from a table 

        EX: SELECT employee-id, device-id
            FROM employees
            ORDER BY employee-id;
  - DESC (Sorting in descending order) ---> The DESC keywork is for "deconding" and tells SQL to sort numbers from largest to smallets, (OR) alphabetically from Z to A.

        EX: SELECT employee-id, device-id
            FROM employees
            ORDER BY employee-id DESC;
- Sorting based on multiple columns ---> We can also choose mutiple columns to ordered. The rows will be sorted for the employee_id. then if multiple values in this row are same. in that case the device_id values will be sourted.

        EX: SELECT employee-id, device-id
            FROM employees
            ORDER BY employee-id , device_id;

### Filter:
The Filtering is one of the most powerful feature of SQL. it is the process of selecting data that match a certain condition.

### Operator:
It is a symbol (or) keyword that represents an Operation.

      EX: country = 'USA'
      
**Syntax** : The rules that determine what is correctly structured in a computing language. To get the full table.

      SELECT * FROM employees;

  
      
