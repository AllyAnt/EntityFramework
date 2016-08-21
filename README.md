# Entity Framework

Entity Framework is an ORM Framework. ORM stands for Object Relational Mapping.
## What is Object Relational Mapping Framework
Object Relational Mapping framework automatically creates classes based on database tables, and the vice versa is also true, that is, it can also automatically generate necessary SQL to create database tables based on classes. 
```sql
Create table Departments
(
     ID int primary key identity,
     Name nvarchar(50),
     Location nvarchar(50)
)

Create table Employees
(
     ID int primary key identity,
     FirstName nvarchar(50),
     LastName nvarchar(50),
     Gender nvarchar(50),
     Salary int,
     DepartmentId int foreign key references Departments(Id)
)
```
