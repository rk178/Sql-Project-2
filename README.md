# Sql-Project-2

Data Analysis of AdventureWorkDW  Database with some queries of table Employeetable 
Dataset :- AdventureWorks 2008 Datawarehousing Database (ms sql)
Url:- https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-serverver15&
tabs=ssms
Database file Name- AdventureworksDW2008.bak (ms sql file)

Used queries:

Q1. Find the title, firstname, ParentEmployeeKey of Employeekey (‘2’) form the table Dimemployee
table present in the database adventurewoksDW2008?
Ans. First select the DimEmployee form the database with below used query
Query used:- select * from DimEmployee;
Then use ‘select’ select columns title,firstname,ParentEmployeeKey form
DimEmployee table where is Employeekey is 2(is the employeekey number to find
the details).
Query Used:-
select Title,FirstName,ParentEmployeeKey from DimEmployee where EmployeeKey In
('2');

Q2.Update ParentEmployeekey of firstname Kevin in the DimEmployee table from the database ?
Ans. First select the Dimemployee table from below query:-
select * from DimEmployee;
Then use update select Dimemployee table set parentemployee to 80 where first name is kevin.
Query used:- UPDATE DimEmployee set ParentEmployeeKey = 80 where FirstName =
'Kevin';



Q3. Find the firstname ‘Rob’ in the DimEmployee table?
Ans. First use select then use DimEmployee where firstname is Rob (Mention firstname rob to find rob in
table)
Query used:-
Select * from DimEmployee where FirstName = 'Rob';




Q4. Do a Right join of two tables form the database?
Ans. Select two tables from database first like in this query:-
SELECT * from DimProduct;
SELECT * from DimProductCategory;
These two tables have common column named as ProductAlternateKey.
Now select both the tables dimproduct and dimproductcategory and right join with
common tables named as ProductAlternateKey.
Below is the query of the above describtion:-
Select * from DimProduct RIGHT JOIN DimProductCategory ON ProductAlternateKey =
ProductAlternateKey;


Q5. Do a inner join from the above tables(Dimproductcategory and Dimproductcategory) in Q4?
Ans. Procedure is same but we have to change query to inner join
Select the tables:-
SELECT * from DimProduct;
SELECT * from DimProductCategory;
Below with used query we can do inner join:-
Select * from DimProduct INNER JOIN DimProductCategory ON ProductAlternateKey =
ProductAlternateKey;
