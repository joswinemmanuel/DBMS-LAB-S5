<h1>ORDER BY, GROUP BY AND HAVING CLAUSE</h1>
AIM:

 Implementation of order by,group by and having clause.

THEORY:

 The ORDER BY command is used to sort the result set in ascending or descending order. The ORDER BY command sorts the result set in ascending order by default. To sort the records in descending order, use the DESC keyword. The GROUP BY statement groups rows that have the same values into summary rows, like "find the number of customers in each country".

 The GROUP BY statement is often used with aggregate functions (COUNT(), MAX(), MIN(), SUM(), AVG()) to group the result-set by one or more columns.

 The HAVING clause was added to SQL because the WHERE keyword cannot be used with aggregate functions.

SYNTAX:

SELECT column_name(s) FROM table_name

WHERE condition

GROUP BY column_name(s)

HAVING condition

ORDER BY column_name(s);

Questions:

·         Create a table Customer (CustomerID , CustomerName, ContactNo, Address, City, PostalCode, Country) with CustomerID as PK

·         Create a table Orders (OrderID, CustomerID, EmployeeID, OrderDate, ShipperID)with OrderID as PK and CustomerID, EmployeeID as FK from Customer and Employee table respectively

·         Create a table Employees (EmployeeID LastName FirstName BirthDate Photo) with EmployeeID as PK

·         Insert 5 tuples in each table

Using ORDER BY:

1.       List all customers in ascending order by their names.

2.       Retrieve a list of orders with the oldest ones appearing first, sorted by order date in ascending order.

3.       Find the employees who were born after 1980 and list them in descending order of their birthdates.

4.       List orders placed by customers from 'USA' in descending order of the order date.

5.       Calculate the total number of orders placed by each customer.

6.       List the cities with the total number of customers.

7.       List customers who have placed more than 2 orders.

8.       Display cities with more than 3 customers.
