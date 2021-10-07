# Problem 

Write an SQL query to print details of the Workers whose FIRST_NAME ends with ‘h’ and contains six alphabets

# Solution

SELECT * FROM Worker
WHERE FIRST_NAME LIKE ('_____h%')