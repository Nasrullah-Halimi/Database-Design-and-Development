# Database
Database Projects completed by me from conceptual model for Academic, self learning and hobby purposes 

The followings provides an overview of how the project

defination of situation:
An educational organization offering computer courses wants to implement a database that would handle the organization data providing 
the following specification 
1.	Keep the attributes minimal for all entities. 
2.	For the instructor entity except for the keys (primary and possible foreign) keep the instructor name
3.	For the subject area, course entities keep only their names.
4.	For the person address keep the street and number, post code and country.
5.	For the offering keep the designated date.
6.	For the organization keep the organization name and tax number (AFM).
7.	For the invoice, keep the invoice date and the amount.
8.	For student keep the name.
9.	For the attendance, no extra attributes are required.


steps taken to desing and implement 

ERD logical model;
An Entity relationship diagram has been devoloped out of the conceptual definition of the situation, you can refer to the file "DB ERD.pdf"
to look up what type of relationship is built between the entities and attributes 

creating database;
based on the ERD the database has been created in Oracle database server envoirnment with the name "DB Define.sql" included in repository
you can take a look to see the relationship between tables, data types etc.. 

insert data;
following the creation of database i have inserted some data via command line, in this repository there is the file "script.txt"
illustrating how the SQL command is used to store data

Quering data using SQL command line:
select distinct Gender from student;
select max (invoice_amount) / 2 from invoice; 
select* from invoice WHERE invoice_amount > 280;
select authorization_no from instructor Group by authorization_no DESC;
Select*from authorization WHERE (authorization_date BETWEEN ‘1981/05/17’ AND ‘1989/12/31’); 







