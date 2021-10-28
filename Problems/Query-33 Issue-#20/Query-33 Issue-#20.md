SELECT * FROM table WHERE salary = 
         (
            SELECT MIN(salary) FROM table 
            WHERE  salary IN (
                                 SELECT DISTINCT TOP N
                                     salary FROM table 
                                         ORDER BY salary DESC
                             )
        )
