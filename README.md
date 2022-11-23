# SQL_Assignment answer
IIHT SQL Day1 Assignment:


 create database Employee;
 create table employee_Details(EMPLOYEE_ID int NOT NULL PRIMARY KEY,FULL_NAME varchar(255),MANAGER_ID int,DATE_JOINING varchar(255),CITY varchar(255));

  Insert into employee_details (EMPLOYEE_ID,FULL_NAME,MANAGER_ID,DATE_JOINING,CITY) values(1,'JOHN',102,22/07/1982,'USA');
  Insert into employee_details (EMPLOYEE_ID,FULL_NAME,MANAGER_ID,DATE_JOINING,CITY) values(2,'PETER',128,22/07/1990,'AUSTRALIA');
  Insert into employee_details (EMPLOYEE_ID,FULL_NAME,MANAGER_ID,DATE_JOINING,CITY) values(3,'Ramesh',102,31/10/2000,'INDIA');
  Insert into employee_details (EMPLOYEE_ID,FULL_NAME,MANAGER_ID,DATE_JOINING,CITY) values(4,'kumar',130,31/10/2020,'INDIA');
  Insert into employee_details (EMPLOYEE_ID,FULL_NAME,MANAGER_ID,DATE_JOINING,CITY) values(5,'Vijay',130,01/12/2021,'INDIA');

QUESTION 1):ans
Select * from employee_details employee_id,full_name where manager_id=130;
Select * from employee_details employee_id,full_name where manager_id=102;


create table employee_salary(EMPLOYEE_ID int NOT NULL PRIMARY KEY,PROJECT varchar(50),SALARY int,VARIABLE int);
insert into  employee_salary(EMPLOYEE_ID,PROJECT ,SALARY,VARIABLE) values(101,'P1',50000,400);
insert into  employee_salary(EMPLOYEE_ID,PROJECT ,SALARY,VARIABLE) values(102,'P2',100000,800);
insert into  employee_salary(EMPLOYEE_ID,PROJECT ,SALARY,VARIABLE) values(103,'P1',150000,800);
insert into  employee_salary(EMPLOYEE_ID,PROJECT ,SALARY,VARIABLE) values(104,'P3',100000,800);
insert into  employee_salary(EMPLOYEE_ID,PROJECT ,SALARY,VARIABLE) values(105,'P3',100000,800);
insert into  employee_salary(EMPLOYEE_ID,PROJECT ,SALARY,VARIABLE) values(106,'P2',80000,200);


QUESTION2):ans
	select * from employee_salary project;

QUESTION3):ans
	select count(project) from employee_salary where project='p1';

QUESTION4):ans
	select min(salary) from employee_salary;

	select max(salary) from employee_salary;

	select avg(salary) from employee_salary;


QUESTION5):ans
	select * from Employee_salary employee_id where salary>9000 AND salary<15000;

	
QUESTION6):ans
	select * from Employee_details full_name where manager_id=321 AND city='Toronto';


QUESTION7):ans
	select * from Employee_details full_name where manager_id=321 OR city='California';


QUESTION8):ans
	select * from Employee_salary full_name where NOT project='P1';


=========================================================================================


QUESTION9):ans
	select * from Employee_details employee_id, full_name where  manager_id='986';


QUESTION2):ans
	select * from  employee_id,SUM(salary+Variable) from employee_salary;

================================================================================================
QUESTION10)ans
	select * from employee_details where full_name LIKE '%hn';
===========================================================================================
QUESTION20)ans
	
