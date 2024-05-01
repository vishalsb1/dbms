# dbms


Insert a single record into the dept table. 
```
create table dept(
dept_id int ,
dept_name varchar(20),
employee_name varchar(20)
);

insert into dept(dept_id,dept_name,employee_name) values(1001,'rajdhani','rajuu lande');

select * from dept;
```
Insert multiple record into the dept table. 
```
create table dept(
dept_id int ,
dept_name varchar(20),
employee_name varchar(20)
);

insert into dept(dept_id,dept_name,employee_name) values(1001,'rajdhani','rajuu lande'),(1001,'rajdhani','rajuu lande'),(1001,'rajdhani','rajuu lande'),(1001,'rajdhani','rajuu lande');

select * from dept;
```
Update the emp table to set the salary of all
employees to Rs15000/- who are working in ASP.
```
create table employee(
emp_id int ,
employee_name varchar(30),
employ_sal int,
emp_dept varchar(20));

insert into employee(emp_id,employee_name,employ_sal,emp_dept) values (1001,'mama',1800,'ASP'), (1101,'mama1',1300,'mech'), (1001,'mama2',4000,'aiml');

select * from employee;

update employee 
set employ_sal=15000
where emp_dept='ASP';

select * from employee;
```
copying a table
```
create table employee(
emp_id int ,
employee_name varchar(30),
employ_sal int,
emp_dept varchar(20));

insert into employee(emp_id,employee_name,employ_sal,emp_dept) values (1001,'mama',1800,'comp'), (1101,'mama1',1300,'mech'), (1001,'mama2',4000,'aiml');

create table emp2 as select * from employee;

select *from emp2;

```
arranging in ascending order 
```
create table employee(
emp_id int ,
employee_name varchar(30),
employ_sal int,
emp_dept varchar(20));

insert into employee(emp_id,employee_name,employ_sal,emp_dept) values (1001,'mama',1800,'comp'), (1101,'mama1',1300,'mech'), (1000,'mama2',4000,'aiml');

create table emp2 as select * from employee;

select * from employee order by emp_id;
```

arrange in descending order 

```
create table employee(
emp_id int ,
employee_name varchar(30),
employ_sal int,
emp_dept varchar(20));

insert into employee(emp_id,employee_name,employ_sal,emp_dept) values (1001,'mama',1800,'comp'), (1101,'mama1',1300,'mech'), (1000,'mama2',4000,'aiml');

select * from employee order by employ_sal desc;
```
select an employee by the id 

```
create table employee(
emp_id int ,
employee_name varchar(30),
employ_sal int,
emp_dept varchar(20));

insert into employee(emp_id,employee_name,employ_sal,emp_dept) values (1001,'mama',1800,'comp'), (1101,'mama1',1300,'mech'), (1000,'mama2',4000,'aiml');

create table emp2 as select * from employee;

select * from employee where emp_id=1001;
```
using distinct keyword
```
create table employee(
emp_id int ,
employee_name varchar(30),
employ_sal int,
emp_dept varchar(20));

insert into employee(emp_id,employee_name,employ_sal,emp_dept) values (1001,'mama',1800,'comp'), (1101,'mama1',1300,'mech'), (1000,'mama2',4000,'aiml');

create table emp2 as select * from employee;

select distinct employ_sal from employee;
```
