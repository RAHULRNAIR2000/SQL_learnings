# SQL_learnings
Details of all SQL queries we are using in daily life 

<h1>Some of The Most Important SQL Commands</h1>

<ul><li>SELECT - extracts data from a database</li>
<li>UPDATE - updates data in a database</li>
<li>DELETE - deletes data from a database</li>
<li>INSERT INTO - inserts new data into a database</li>
<li>CREATE DATABASE - creates a new database</li>
<li>ALTER DATABASE - modifies a database</li>
<li>CREATE TABLE - creates a new table</li>
<li>ALTER TABLE - modifies a table</li>
<li>DROP TABLE - deletes a table</li>
<li>CREATE INDEX - creates an index (search key)</li>
<li>DROP INDEX - deletes an index</li>
</ul>

<h2>SELECT Syntax</h2>
SELECT column1, column2, ...
FROM table_name;

SELECT * FROM table_name;

<h2>SELECT DISTINCT Syntax</h2>

SELECT DISTINCT column1, column2, ...
FROM table_name;

<h2>Findng Count example</h2>

SELECT COUNT(DISTINCT Country) FROM Customers;

<h2>WHERE Syntax</h2>

SELECT column1, column2, ...
FROM table_name
WHERE condition;

<h2>Operators in The WHERE Clause</h2>

= 	Equal	

 >	 Greater than	

<	 Less than
	
>=  	Greater than or equal	

<=	 Less than or equal	

<>	 Not equal. Note: In some versions of SQL this operator may be written as !=	

BETWEEN	 Between a certain range	

LIKE	 Search for a pattern	

IN	  To specify multiple possible values for a column	

<h2>The MySQL AND, OR and NOT Operators </h2>

AND Example

SELECT * FROM Customers
WHERE Country = 'Germany' AND City = 'Berlin';

OR Example

SELECT * FROM Customers
WHERE City = 'Berlin' OR City = 'Stuttgart';

NOT Example

SELECT * FROM Customers
WHERE NOT Country = 'Germany';

<h2>The MySQL ORDER BY Keyword</h2>

The ORDER BY keyword is used to sort the result-set in ascending or descending order.

The ORDER BY keyword sorts the records in ascending order by default. To sort the records in descending order, use the DESC keyword.

SELECT * FROM Customers
ORDER BY Country;

SELECT * FROM Customers
ORDER BY Country DESC;

