<h1>IMPLEMENTATION OF SET OPERATORS, NESTED QUERIES AND JOIN QUERIE</h1>
AIM: To implement set operators, nested queries and join queries in SQL.

 THEORY: SET operators are special types of operators which are used to combine the result of two queries. Operator
s covered under SET operators are

: UNION 

UNION ALL 

INTERSECT 

MINUS 

A Subquery or Inner query or a Nested query is a query within another SQL query and embedded within the WHERE clause. A subquery is used to return data that will be used in the main query as a condition to further restrict the data to be retrieved. Subqueries can be used with the SELECT, INSERT, UPDATE, and DELETE statements along with the operators like =, <, >, >=, <=, IN, BETWEEN, etc. 

A JOIN clause is used to combine rows from two or more tables, based on a related column between them.

 Questions: 

Amazon is one of the largest online stores operating in the United States of America. They are maintaining four tables in their database.

 The Items table, Customers table, Orders table and Delivery table. Each of these tables contains the following attributes:

 1. Items: - itemid (primary key) Itemname(type =varchar(50)) 50 category Price Instock (type=int, greater than or equal to zero) 

2. Customers:- custid (primary key) Custname Address state 

3. Orders:- orderid (primary key) Itemid( refers to itemid of Items table) Custid (refers to custid in customers table) Quantity (type=int) Orderdate (type=date) 

4. Delivery:- deliveryid (primary key) Custid (refers to custid in customers table) Orderid (refers to ordered in orders table)

 1. List the details of all customers who have placed an order

 2. List the details of all customers whose orders have been delivered

 3. Find the order date for all customers whose name starts in the letter ‘s’ 

4. Display the name and price of all items bought by the customer ‘Elvin’

 5. List the details of all customers who have placed an order after January 2013 and not received delivery of items

 6. Find the itemid of items which has either been ordered or not delivered. (UseSET UNION)

 7. Find the name of all customers who have placed an order and have their orders 

8. Find the custname of all customers who have placed an order but not having their orders delivered. (Use SET MINUS) delivered.(Use SET INTERSECTION) 

 9. Find the name of the customer who has placed the most number of orders.

 10. Find the details of all customers who have purchased items exceeding a price of 5000$ 

11. Find the name and address of customers who has not ordered a ‘Samsung GalaxyS4’ 

12. Perform Left Outer Join and Right Outer Join on Customers & Orders Table. 
