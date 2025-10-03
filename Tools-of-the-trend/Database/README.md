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
- WHERE ---> It indicates the condition for a filter.

        # To Get the colums that present in USA. we can use
  
        EX: SELECT *
            FROM employees
            WHERE office = 'USA';

- LIKE ---> It is an operator used with "WHERE" to search for pattern in a column.

        # here we are looking for values that starts with EAST
  
        EX: SELECT *
            FROM employees
            WHERE office LIKE 'EAST%'; 
- BETWEEN ---> An operator that filters for numbers (or) dates within a range.

        EX: SELECT *
            FROM employees
            WHERE Patch-date BETWEEN '2021-03-01' AND '2021-09-01';

## Logical Operators
AND, OR, and NOT allow us to filter our queries to return the Specific information that will help us.
    
- AND ---> It specifices that both conditions must be met simultaneously. in AND operator we should meet both the conditions then only the value is displayed.

        EX: SELECT *
            FROM machines
            WHERE operating-sys = 'OS1' AND email = 'Email 1';
  
- OR ---> it specifies that either condition can be met, The values can meet first condition (OR) second condition are it can work if both conditions meet.

        EX: SELECT *
            FROM machines
            WHERE operating-sys = 'OS1' OR operating-sys = 'OS3';
  
- NOT ---> It negates a condition. it looks for an entry that does not match the condition we specified.

        EX: SELECT *
            FROM machines
            WHERE NOT operating-sys = 'OS3';

**Combining logical operators** : logical operators can be combined in filter. If we want customers in other contries apart from canada & USA.

        SELECT firstname, lastnumber, email,country
        FROM customers
        WHERE NOT country = 'canada' AND NOT contry = 'USA';

### Filter:
The Filtering is one of the most powerful feature of SQL. it is the process of selecting data that match a certain condition.

### Operator:
It is a symbol (or) keyword that represents an Operation.

      EX: country = 'USA'
      
**Syntax** : The rules that determine what is correctly structured in a computing language. To get the full table.

      SELECT * FROM employees;

**Patterns** : We can search the columns with proper patterns.

        a%   ---> art, a, apple
        a_   ---> as, an
        a_ _ ---> ant, add
        %a   ---> Pizza, Tina
        _a   ---> ma, la
        %a%  ---> again, back
        _a_  ---> car, ban

The Three common data types found in databases.
    
  - String
  - Numberic
  - data and time
      
**String** : It is a data Consisting of an ordered sequence of characters. This can be numbers, letters, and symbols.

      username = analyst10

**Numberic data** : it is the data consisting of numbers, such as count of log in attempts. unlike string ,mathematical operations can be performed on number data.

**Date and Time data** : Data representing a data and /or time.

## Common Operators for working with numeric & data and time data
  
    Operation:  =, > ,< , < >, >=, <=

    EX: SELECT *
        FROM log_in
        WHERE time > '18:00';

## JOIN 
This helps when we need information from two different tables in a database. since we will be working with two tables, we need a way to tell SQL what table we picking. To join two tables we need to identify the shared common column between those two tables. Now we can connect them using a primary key and foreign key setup.
          
          <Table_name>.<column_name>

        Ex: employees.employee_id & machines.employee_id

**NULL values** : Thsi can be values that are not assigned. it represents a missing value due to any reason.

**Primary Key**: 
It is a column in a database table that uniquely identifies each row in that table.

**Characteristics**
  
  - **Unique** : No two rows can have same values
  - **Not Null** : The values can not be Null
  - **Immutable** : The Values of the key cannot change

**Foreign Key**:
it is a column in one table that refers to the primary key in another table. It is used to link two tables together.

### Type of Join

- **INNER JOIN** : This returns rows matching on a specified column that exists in more than one table. With this common key pairs will be collected and the data in those columns will be combined into a single table.

      EX: SELECT username, office, OS
          FROM emp
          INNER JOIN mac ON emp.emp_id = mac.emp_id;
  
- **OUTER JOIN** : They are used to Combine rows from two (or) more tables based on a related column, and importantly , they include rows that do not have a match in the other tables.

### Type of outer joints

- **LEFT JOIN** : It returns all of the records of the first table, but only returns rows of the second table that match on a specified column.
- **SELF JOIN** : It is when a table is joined to itself. we can treat it like two separate tables to compare or relate rows within the same table.
- **RIGHT JOIN** : It returns all of the records of the second table, but only returns rows from the first table that match on a specified column.
- **FULL OUTER JOIN** : This will returns all records from both tables. if a row dont have any value for a column then it will return as null.

Similar to inner join, outer join combine two tables together

### Aggregate funtions
These are funtions that perform a calculationover multiple data points & return the result of the calculation.Some of the aggregate funtions are

  - Count  ---> Returns a number that shows number of rows from the query.
  - AVG    ---> Returns a number that shows avg of the numeric data in column.
  - SUM    ---> Returns a number that shows sum of numbers in a column.

**Syntax**:

      count --> SELECT COUNT (name) FROM Customer;
      
      Avg   --> SELECT AVG (name) FROM Customer;

      sum   --> SELECT SUM (name) FROM customer;
