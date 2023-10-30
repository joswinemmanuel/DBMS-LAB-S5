<h1>CREATION OF VIEWS AND ASSERTIONS</h1>
AIM: 

To create views and assertions. 

THEORY: 

Views in SQL 

Views in SQL are considered as a virtual table. 

A view also contains rows and columns.

 To create the view, we can select the fields from one or more tables present in the database. 

A view can either have specific rows based on certain conditions or all the rows of a table. 

An assertion is a statement in SQL that ensures a certain condition will always exist in the database. Assertions are like column and table constraints, except that they are specified separately from table definitions.



Questions: 

i)Create a table named Bank with the following attributes 

-bankcode (To be set as Primary Key, type= varchar(3)) 

-bankname (Should not beNULL) 

-headoffice 

-branches (Integer value greater tha nZero) 

Populate the database. 

Make sure that all constraints are working properly. 

All constraints have to be set after creating the table.

ii)Create a table named Branch with the following attribute

-branchid (To be set as PrimaryKey)

-branchname (Set Default value as ‘New Delhi’) 

bankid (Foreign Key:- Refers to bank code of Bank table)

Populate the database. Make sure that all constraints are working properly

iii) Delete the bank with bank code ‘SBT’ and make sure that the corresponding entries are getting deleted from the related tables.

iv) Drop the Primary Key in branch using ALTER command

v) Create a View named bank_head office to hold the details of all bank whose head office at Ernakulam.

vi) Create a View named bank_branch to hold the details of all bank who have branches at kottayam.



RESULT: Creation of views and assertions have been done and the output has been verified and CO2 is attained.
