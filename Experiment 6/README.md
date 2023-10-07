<h1>Implementation of Built-in functions in RDBMS using temp tables</h1>

AIM:

To implement built in functions in RDBMS using temp tables.

 THEORY:

SQRT- Returns the square root of a given non-negative number.

 CONCAT- Adds two or more strings together.

LENGTH- Returns the length of a string.

REVERSE- Reverses a string and returns the value.

FLOOR- This function rounds the specified number down and returns the largest number that is less than or equal to the specified number.

CEIL- This function rounds the specified number up and returns the smallest number that is greater than or equal to the specified number.

ABS- Returns the absolute value of a number.

Ltrim,Rtrim-  The LTRIM (left trim) and RTRIM (right trim) functions allow you to remove specified characters from a string’s left or right side, respectively.

Rpad- functions are used to pad a string with a specified character to the  right. To use the RPAD function, you pass in the string you want to pad, the desired length of the padded string, and the character you want to pad with as arguments and the function will return the padded string. 

substring- It allows the user to extract a specified string portion. 

QUERIES             

Use the system table DUAL for the following questions

1.       Find the Ceil value of 8.29

2.       Round up -3.9 using the CEIL function.

3.       Ceil the result of 17 divided by 3.

4.       Find the floor value of 9.76

5.       Round down -5.3 using the FLOOR function.

6.       Floor the result of 15 divided by 4.

7.        Find the square root of 625

8.       Calculate the square root of 2 using the SQRT function.

9.        Find the abs value of 8.29

10.   Find the absolute value of a negative number, - 3.14.

11.   Determine the absolute value of a numeric column, -42.

12.   Display the current date (set for the operating system on which the database server resides) using SYSDATE as NOW

13.   Use To_Char egg to display date and time in different formats

14.   Display system date and time using SYSTIMESTAMP 

15.   Demonstrate the use of LEAST function in string, by passing three strings as arguments

16.   Demonstrate the use of GREATEST function in string, by passing three strings as arguments

17.   Remove leading spaces from the string '        Trim me'.

18.   Remove Trailing spaces from the string ‘I love India                '.

19.   Right-pad your own name to be 15 characters long with 'X'.

20.   Right-pad a numeric column, e.g., 123, with zeros to make it 6 characters long.

21.   Display the reverese of the string 'uoy evol I'

22.   Reverse the string 'racecar' to check if it's a palindrome.

23.   Find the length of the string 'Oracle Database'.

24.   Concatenate the following strings: 'Oracle', 'SQL', 'is', 'powerful', and 'flexible'.

25.   Concatenate your first name and last name using concat function

26.   Use SUBSTR function to retrieve the substring ‘is’ from the string ‘India is my country’

27.   Extract a substring of your own name, the middle 3 characters.

28.   Extract the first 3 characters from the string 'Substring'.

PART B

Create a table named angle with the trigonometric functions in the first row such as sin, cos, tan,cot , sec and  insert angles such as 0°, 30°, 45°, 60°, 90°, and find all 


Hints :
create table angle
insert into angle(angle) values(0);
....
....

UPDATE angle SET sin=sin(angle*(3.14/180));
