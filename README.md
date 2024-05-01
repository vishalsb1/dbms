# dbms


-- Insert a single record into the dept table. 

```create table dept(
dept_id int ,
dept_name varchar(20),
employee_name varchar(20)
);

insert into dept(dept_id,dept_name,employee_name) values(1001,'rajdhani','rajuu lande');

select * from dept;
