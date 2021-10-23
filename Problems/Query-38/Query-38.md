SELECT  *
     FROM Worker
     LEFT JOIN Bonus
     ON worker.WORKER_REF_ID=Bonus.WORKER_REF_ID
INTERSECT
    SELECT  *
     FROM Worker
     RIGHT JOIN Bonus
     ON worker.WORKER_REF_ID=Bonus.WORKER_REF_ID;