### 1. For Table - Worker
select * from 
    (select 
        WORKER_ID, 
        FIRST_NAME, 
        LAST_NAME, 
        SALARY,
        JOINING_DATE, 
        DEPARTMENT, 
        rownum rm 
    from 
        Worker)
where mod(rm, 2)=0;

### 2. For Table - Bonus
select * from
    (select 
        WORKER_REF_ID, 
        BONUS_DATE, 
        BONUS_AMOUNT, 
        rownum rm 
    from 
        Worker)
where mod(rm, 2)=0;

### 3. For Table - Title
select * from
    (select 
        WORKER_REF_ID,
        WORKER_TITLE, 
        AFFECTED_FROM, 
        rownum rm 
    from 
        Worker)
where mod(rm, 2)=0;
