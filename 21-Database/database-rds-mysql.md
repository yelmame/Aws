
# Database
A database is a structured place to store, organize, and retrieve data
kind of like a super-organized digital filing cabinet.
Instead of keeping notes on paper or scattered files on your computer, a database stores information in a way that’s easy for computers (and people) to access, search, and update efficiently. 

## Types of Databases: 

### 1. Relational Databases (SQL) – Like MySQL, PostgreSQL, Oracle 

Use tables (rows + columns) 

Require a fixed structure (schema) 

### 2. NoSQL Databases – Like MongoDB, DynamoDB, Firebase 

More flexible, store data as documents, key-value pairs, etc. 

Great for unstructured or fast-changing data 

## configuration of RDS(relational database ) in  aws
    `bash 
    Create  a Relational database in AWS as RDS service  

    Step1:
    choose a database creation method 

    Standard create  

    Configuration : MYSQL  

    Db Instance size : Free tier 

    DB instance identifier: database1 

    Master username: admin 

    Password: redhat#123 

    Step2:
    setup ec2 connection  

    Create db class (burstable class) 

    Connectivity 

    dont connect to ec2 instance  

    connect to default vpc  

    public access – yes  

    vpc security group  : default security group  

    Availabity zone : no preference  

    Certificate authority : default  

    Additional configuration : select port 3306 

    Database authentication : password authentication  

    Monitoring: database insight standard  

    Additional configuration setting : 

    database name : enter the name of database  

    backup  

    Encryption  

    Create a database  

 `

 how to access the database 

 type1:
  
 install mysql workbench 
 connect to database with database endpoint & username password
 run mysql commands 

 mysql commands

1 create database redhat;

2 show databases;

3 use redhat;

4 create table school(rollno int, name varchar(20), subject varchar(30));

5 select * from school;

6 insert into school(rollno, name, subject) values(01, "manager", "computer");

7 insert into school(rollno, name, subject) values(02, "rahul", "math");

type2 : access database throgh ec2 instance 

create ec2 instance & add 3306 port allow

create database connectivity with ec2 instance

ec2 instance :

yum install mariadb*

yum install mysql*

mysql -u admin -h database-endpoint -p

MySQL >show databases;

>use command 


