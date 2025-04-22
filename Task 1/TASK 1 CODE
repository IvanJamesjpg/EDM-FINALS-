DROP database multilevel_company;
create DATABASE multilevel_company;
USE multilevel_company;
##task 1
create table employees(
employee_id INT auto_increment primary key,
employee_name varchar(255) NOT NULL,
manager_id INT,
foreign key (manager_id) references employees(employee_id) ON UPDATE CASCADE
);

describe employees;
##task 2

create table departments (
department_id INT auto_increment primary key,
department_name varchar (255) NOT NULL
);
describe departments;

##task3

create table employee_departments(
employee_id INT,
department_id INT,
PRIMARY KEY (employee_id,department_id),
foreign key (employee_id) references employees (employee_id) ON update cascade,
foreign key (department_id) references departments (department_id) ON update cascade
);

DROP TABLE employee_departments;

##TASK4
create table employee_projects(
employee_id INT auto_increment primary key,
project_name varchar(255) NOT NULL
);

describe employee_projects;
##TASK5 

create table managers (
manager_id INT auto_increment primary key,
employee_id INT,
foreign key (employee_id) references employees (employee_id) on update cascade
);
describe managers;

show databases;
