# Problem 

Write an SQL query to fetch the names of workers who earn the highest salary

# Solution

SELECT * FROM Worker ORDER BY SALARY DESC
SELECT MAX(SALARY) FROM Worker