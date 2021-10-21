## Query to 5th highest salary

`
SELECT FirstName, Salary 
FROM Worker w1
WHERE 5-1 = (SELECT COUNT(DISTINCT Salary) FROM Worker w2
WHERE w2.Salary > w1.Salary)
`