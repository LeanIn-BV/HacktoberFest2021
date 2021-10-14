-- Replace N with the number of max salaries you want to fetch from Worker table
SELECT w1.first_name, w1.last_name, w1.salary FROM Worker w1 ORDER BY salary DESC LIMIT N;