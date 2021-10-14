## By selecting each column individually:-

`Select FIRST_NAME , LAST_NAME , SALARY from Worker where SALARY >=50000 and SALARY <=100000; `

## By concatenate two columns:-

`Select concat(FIRST_NAME , ' ' , LAST_NAME) as Name , SALARY from Worker where SALARY >=50000 and SALARY <=100000;`