SELECT w1.first_name, w1.last_name, w1.salary, w1.department
FROM Worker w1
INNER JOIN Worker w2 ON w1.salary = w2.salary AND w1.worker_id <> w2.worker_id;