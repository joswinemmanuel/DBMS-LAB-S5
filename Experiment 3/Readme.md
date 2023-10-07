<h1>DDL(Data Definition Language) Commands</h1>

Aim: To study the database initialization and DDL commands such as Create,Alter,Truncate,Drop.

Theory: 

CREATE – Create an object. I mean, create a database, table, triggers, index, functions, stored procedures, etc. 
DROP – This SQL DDL command helps to delete objects. For example, delete tables, delete a database, etc. 
ALTER – Used to alter the existing database or its object structures. 
TRUNCATE – This SQL DDL command removes records from tables 5. RENAME – Renaming the database objects 
Write SQL commands to: 

Create a database by named Library 
Create DDL statements and create the tables and constraints (from the design) in the database created (ie. Library) 
Insert values to each table as per the requirement stated below
BOOK (Book_Id, Title, Language_Id, MRP, Publisher_Id, Published_Date, Volume, Status) // Language_Id, Publisher_Id are FK (Foreign Key)

AUTHOR(Author_Id, Name, Email, Phone_Number, Status)

BOOK_AUTHOR(Book_Id, Author_Id) // many-to-many relationship, both columns are PKFK (Primary Key and Foreign Key)

PUBLISHER(Publisher_id, Name, Address)

MEMBER(Member_Id, Name, Branch_Code, Roll_Number, Phone_Number, Email_Id, Date_of_Join, Status)

BOOK_ISSUE(Issue_Id, Date_Of_Issue, Book_Id, Member_Id, Expected_Date_Of_Return, Status) // Book+Id and Member_Id are FKs

BOOK_RETURN(Issue_Id, Actual_Date_Of_Return, LateDays, LateFee) // Issue_Id is PK and FK

LANGUAGE(Language_id, Name) //Static Table for storing permanent data LATE_FEE_RULE(FromDays, ToDays, Amount) // Composite Key

The requirement: A library wants to maintain the record of books, members, book issue, book return, and fines collected for late returns, in a database. The database can be loaded with book information. Students can register with the library to be a member. Books can be issued to students with a valid library membership. A student can keep an issued book with him/her for a maximum period of two weeks from the date of issue, beyond which a fine will be charged. Fine is calculated based on the delay in days of return. For 0-7 days: Rs 10, For 7 – 30 days: Rs 100, and for days above 30 days: Rs 10 will be charged per day.

Questions :

4. Alter Table - Add a new column ISBN to the BOOK table:

5. Alter Table - Modify the data type of a column roll_number  in the MEMBER table:

6. Truncate Table - Remove all records from the PUBLISHER table:

Note: In Oracle, you cannot directly use the TRUNCATE TABLE command without disabling referential constraints. If there are foreign key constraints referencing the table you want to truncate, Oracle won't allow truncation.

7. Drop Table - Delete the AUTHOR table from the database:

8. Rename Table - Change the name of the LATE_FEE_RULE table to  FINE table
