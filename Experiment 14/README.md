<h1>Experiment 14 : CREATIONS OF PROCEDURES,TRIGGERS AND FUNCTIONS.</h1>
AIM:

To create Procedures, Triggers and Functions in PL/SQL Program.

THEORY:

Procedures − These subprograms do not return a value directly; mainly used to perform an action.



CREATE [OR REPLACE] PROCEDURE procedure_name

[ (parameter [,parameter]) ]

IS

[declaration_section]

BEGIN

executable_section

[EXCEPTION

exception_section]

END [procedure_name];

Triggers are stored programs, which are automatically executed or fired when some events occur.

Triggers are, in fact, written to be executed in response to any of the following events −

● A database manipulation (DML) statement (DELETE, INSERT, or UPDATE)

● A database definition (DDL) statement (CREATE, ALTER, or DROP).

● A database operation (SERVERERROR, LOGON, LOGOFF, STARTUP, or SHUTDOWN).



CREATE [OR REPLACE ] TRIGGER trigger_name

{BEFORE | AFTER | INSTEAD OF }

{INSERT [OR] | UPDATE [OR] | DELETE}

[OF col_name]

ON table_name

[REFERENCING OLD AS o NEW AS n]

[FOR EACH ROW]

WHEN (condition)

DECLARE

Declaration-statements

BEGIN

Executable-statements

EXCEPTION

A standalone function is created using the CREATE FUNCTION statement. The simplified syntax for

the CREATE OR REPLACE PROCEDURE statement is as follows −

CREATE [OR REPLACE] FUNCTION function_name

[(parameter_name [IN | OUT | IN OUT] type [, ...])]

RETURN return_datatype

{IS | AS}

BEGIN

< function_body >

END [function_name];

Questions:

Procedures and Functions

1. Create a function factorial to find the factorial of a number. Use this function in PL/SQL Program

to display the factorial of a number read from the user.

2. Create a table student_details (roll int, marks int, phone int). Create a procedure pr1 to update

all rows in the database. Boost the marks of all students by 5%.

3. Create a table student (id, name, m1, m2, m3, total, grade). Create a function f1 to calculate

grade. Create a procedure p1 to update the total and grade.

• Read: id, name, m1, m2, m3 from the user

•Insert the tuple into the database

•Using function f1 calculate the grade

•Using procedure p1, update the grade value for the tuple

Trigger

Write PL/SQL programs for the following:

Create a table customer_details (cust_id (unique), cust_name, address).

Create a table emp_details (empid (unique), empname, salary)

Create a table cust_count (count_row)

1) Create a trigger whenever a new record is inserted in the customer_details table.

2) Create a trigger to display a message when a user enters a value > 20000 in the salary

field of emp_details table.

3) Create a trigger w.r.t customer_details table. Increment the value of count_row (in

cust_count table) whenever a new tuple is inserted and decrement the value of

count_row when a tuple is deleted. Initial value of the count_row is set to 0.

4) Create a trigger to insert the deleted rows from emp_details to another table and

updated rows to another table. (Create the tables deleted and updated)
