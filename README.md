# Ex-No-4-Creating-Procedures-using-PL-SQL
AIM:
To create a procedure using PL/SQL.

Steps:
Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
Create a procedure named as insert_employee data.
Inside the procdure block, write the query for inserting the values into the employee table.
End the procedure.
Call the insert_employee data procedure to insert the values into the employee table.
Display the employee table
Program:
SQL> create table employeee(empid number,empname varchar (20), dept varchar (10) ,salary number);

Table created.

SQL> create or replace procedure insert_employeee_data AS
  2  begin
  3  insert into employeee (empid,empname,dept,salary)
  4  values (1,'NANDHA','MD',1000000);
  5  insert into employeee (empid,empname,dept,salary)
  6  values (2,'ROHIT','HR',500000);
  7  insert into employeee (empid,empname,dept,salary)
  8  values (3,'TEJUS','IT',200000);
  9  commit;
 10  end;
 11  /

Procedure created.

SQL> begin
  2  insert_employeee_data;
  3  end;
  4  /

PL/SQL procedure successfully completed.

SQL> select * from employeee;
Output:
Screenshot 2023-09-28 222242

Result:
Hence the procedure using pl/sql is created successfully.
