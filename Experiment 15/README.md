<h1>EXPERIMENT- 15 CREATION OF PACKAGES </h1>
AIM: To implement Packages


THEORY: 

A package is a schema object that groups logically related PL/SQL types, variables, constants, subprograms, cursors, and exceptions. 

A package is compiled and stored in the database, where many applications can share its contents. 

CREATE [OR REPLACE] PACKAGE AS 

<sub_program and public element declaration>

END <package name>

STEPS:
1) CREATE PACKAGE SPECIFICATION
2)PACKAGE BODY
3)Use this package in a PL/SQL program.
Call the functions  and procedures within the program and display their result

Question:Assignment

Create a package pk1 consisting of the following functions and procedures

Procedure proc1 to find the sum, average and product of two numbers

Procedure proc2 to find the square root of a number

Function named fn11 to check whether a number is even or not

A function named fn22 to find the sum of 3 numbers

Use this package in a PL/SQL program. Call the functions f11, f22 and procedures pro1, pro2 within the program and display their result
