Project description:
An educational organization offering computer courses wants to implement a database that would handle the organization data with the following specifications;
1.	Keep the attributes minimal for all entities. 
2.	For the instructor entity except for the keys (primary and possible foreign) keep the instructor name.
3.	For the subject area, course entities keep only their names.
4.	For the person address keep the street and number, post code and country.
5.	For the offering keep the designated date.
6.	For the organization keep the organization name and tax number (AFM).
7.	For the invoice, keep the invoice date and the amount.
8.	For student keep the name.
9.	For the attendance, no extra attributes are required.


The following steps taken to design and implement the database.

ERD logical model: an entity relationship diagram (ERD) has been devoloped out of the conceptual definition of the situation, refer to "DB ERD.pdf" file
for type of relationship built between the entities and attributes.

Creating database: based on the ERD the database has been created in Oracle database server envoirnment with the name "DB Define.sql".

Inserting data: some data inserted via command line, the "script.txt" illustrates how SQL command is used to store data.

Quering data using SQL command line.
1. select distinct Gender from student;
2. select max (invoice_amount) / 2 from invoice; 
3. select * from invoice WHERE invoice_amount > 280;
4. select authorization_no from instructor Group by authorization_no DESC;
5. Select * from authorization WHERE (authorization_date BETWEEN ‘1981/05/17’ AND ‘1989/12/31’); 
