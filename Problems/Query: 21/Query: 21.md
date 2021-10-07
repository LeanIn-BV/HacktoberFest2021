# Problem
Write an SQL query to fetch the count of employees working in the department ‘Admin’.

# Solution  
```sql
SELECT COUNT(WORKER_ID) FROM Worker WHERE DEPARTMENT = 'Admin' 
```
