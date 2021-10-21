SELECT * FROM Employee WHERE sal = 
         (
            SELECT MIN(sal) FROM Employee 
            WHERE  sal IN (
                                 SELECT DISTINCT TOP N
                                     sal FROM Employee 
                                         ORDER BY sal DESC
                             )
        )
