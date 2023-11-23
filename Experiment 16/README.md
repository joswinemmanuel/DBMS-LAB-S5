<h1>EXPERIMENT 16 : CREATION OF CURSORS</h1>
AIM:

To create a Cursor.

THEORY:

In Oracle PL/SQL, a cursor is a named private SQL area from where information can be accessed. It is used to process individual rows returned by a SQL query. Cursors provide a way to iterate over a set of rows returned by a query, allowing you to perform operations on each row one at a time.

A cursor is a pointer to this context area. PL/SQL controls the context area through a cursor. A cursor holds the rows (one or more) returned by a SQL statement. The set of rows the cursor holds is referred to as the active set. There are two types of cursors in Oracle PL/SQL: implicit and explicit.

Implicit Cursors:

These are automatically created by Oracle when a SQL statement is executed.There is no need to declare or define implicit cursors.

Examples of implicit cursors include SQL%ROWCOUNT (returns the number of rows affected by the last SQL statement) and SQL%FOUND (returns TRUE if the last SQL statement returned at least one row).

Example:

DECLARE

   emp_count NUMBER;

BEGIN

   SELECT COUNT(*) INTO emp_count FROM employees WHERE department_id = 10;

   DBMS_OUTPUT.PUT_LINE('Number of employees in department 10: ' || emp_count);

END;

Explicit Cursors:

These are created and managed by the user.Explicit cursors give you more control over the processing of query results.You need to declare, open, fetch, and close explicit cursors.

DECLARE variables;

records;

create a cursor;

BEGIN

OPEN cursor;

FETCH cursor;

process the records;

CLOSE cursor;

END;

 

 

 

EXAMPLE

DECLARE

//cursor name as emp_cursor

   CURSOR emp_cursor IS

//SQL Query in declare block

      SELECT employee_id, first_name, last_name FROM employees WHERE department_id = 10;

//a variable declaration for each emp_rec for accessing the row by row data from the named cursor

      emp_rec emp_cursor%ROWTYPE;

BEGIN

   OPEN emp_cursor;

   LOOP

      FETCH emp_cursor INTO emp_rec;

      EXIT WHEN emp_cursor%NOTFOUND;

      DBMS_OUTPUT.PUT_LINE('Employee ID: ' || emp_rec.employee_id || ', Name: ' || emp_rec.first_name || ' ' || emp_rec.last_name);

   END LOOP;

   CLOSE emp_cursor;

END;

In this example:

CURSOR emp_cursor is declared to hold the result set of a query.

emp_cursor%ROWTYPE is used to declare a record that has the same structure as the rows in the cursor.

OPEN, FETCH, and CLOSE statements are used to manipulate the cursor.

Cursor Attributes:

%FOUND: Returns TRUE if a cursor has fetched at least one row.

%NOTFOUND: Returns TRUE if a cursor has not fetched any rows.

%ROWCOUNT: Returns the number of rows fetched by a cursor.

 

 

QUESTIONS

1)Create bank_details (accno, name, balance, adate) Table.

 Calculate the interest of the amount and insert into a new table with fields (accno, interest). Interest= 0.08*balance.


2) Create a table student (id, name, m1, m2, m3, grade). Insert 5 tuples into it. Find the total,

calculate grade and update the grade in the table.


3) Create table people_list (id, name, dt_joining, place). If person’s experience is above 10 years, put the tuple in table exp_list (id, name, experience).


4. Create table employee_list(id,name,monthly salary).

If:annual salary&lt;60000, increment monthly salary by 25%

between 60000 and 200000, increment by 20%

between 200000 and 500000, increment by 15%


annual salary&gt;500000, increment monthly salary by 10%

RESULT:

Creation of the cursor is completed successfully and CO3 is attained.
