 -- SQL query to print details for Workers with the first name as “Vipul” and “Satish” from Worker table

-- creating table
CREATE TABLE Worker(  
Worker_ID Bigint(15),
First_Name Varchar(100),
Last_Name Varchar(100),
Salary Bigint(15),
joining_date datetime,
department Varchar(100));

-- Inserting values in table
INSERT INTO Worker (Worker_ID,First_Name,Last_Name,Salary,joining_date,department) VALUES ('001', 'Monika', 'Arora', '100000', '2014-02-20 09:00:00', 'HR');
INSERT INTO Worker (Worker_ID,First_Name,Last_Name,Salary,joining_date,department) VALUES ('002', 'Niharika', 'Verma', '80000', '2014-06-11 09:00:00', 'Admin');
INSERT INTO Worker (Worker_ID,First_Name,Last_Name,Salary,joining_date,department) VALUES ('003', 'Vishal', 'Singhal', '300000', '2014-02-20 09:00:00', 'HR');
INSERT INTO Worker (Worker_ID,First_Name,Last_Name,Salary,joining_date,department) VALUES ('004', 'Amitabh', 'Singh', '500000', '2014-012-20 09:00:00', 'Admin');
INSERT INTO Worker (Worker_ID,First_Name,Last_Name,Salary,joining_date,department) VALUES ('005', 'Vivek', 'Bhati', '500000', '2014-06-11 09:00:00', 'Admin');
INSERT INTO Worker (Worker_ID,First_Name,Last_Name,Salary,joining_date,department) VALUES ('006', 'Vipul', 'Diwan', '200000', '2014-06-11 09:00:00', 'Account');
INSERT INTO Worker (Worker_ID,First_Name,Last_Name,Salary,joining_date,department) VALUES ('007', 'Satish', 'Kumar', '75000', '2014-01-20 09:00:00', 'Account');
INSERT INTO Worker (Worker_ID,First_Name,Last_Name,Salary,joining_date,department) VALUES ('008', 'Geetika', 'Chauhan', '90000', '2014-04-11 09:00:00', 'Admin');

-- query: 13 Solution
Select * from Worker
where First_Name = 'Vipul' or First_Name = 'Satish'
