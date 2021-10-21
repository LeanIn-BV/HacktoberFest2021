⭐ Request Type
Write an SQL query to fetch the no. of workers for each department in descending order.

## Solution

SELECT DEPARTMENT, count(WORKER_ID) AS No_Of_Workers  
FROM worker  
GROUP BY DEPARTMENT   
ORDER BY No_Of_Workers DESC;