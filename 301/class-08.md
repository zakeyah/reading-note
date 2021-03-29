# SQL 

![](https://i1.wp.com/brianbonk.dk/wp-content/uploads/2021/02/sql-server-tips.jpg?fit=1200%2C500&ssl=1)
## What is SQL?

+ ***SQL***  stands for : Structured Query Language

+ It is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database.

+ It provide safe and scalable storage for millions of websites and mobile applications.

## Relational databases

+ A relational database represents a collection of related (two-dimensional) tables.  with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.

## SELECT queries 

+ To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially referred to as queries.

+ the most basic query we could write would be one that selects for a couple columns (properties) of the table with all the rows (instances).

*Select query for a specific columns* :

- SELECT *column*, *another_column*, etc...
- FROM mytable;

"two-dimensional set of rows and columns, effectively a copy of the table, but only with the columns that we requested."

*Select query for all columns*

- SELECT * 
- FROM mytable;

"inspect a table by dumping all the data at once."

## Queries with constraints P1

+ In order to filter certain results from being returned, we need to use a WHERE clause in the query.

*Select query with constraints* :

- SELECT column, another_column, …
- FROM mytable
- WHERE condition
    - AND/OR another_condition
    - AND/OR …;

"More complex clauses can be constructed by joining numerous AND or OR logical keywords"

## Queries with constraints P2

When writing WHERE clauses with columns containing text data, SQL supports a number of useful operators to do things like case-insensitive string comparison and wildcard pattern matching. 

*All strings must be quoted so that the query parser can distinguish words in the string from SQL keywords.*

## Filtering and sorting Query results

Even though the data in a database may be unique, the results of any particular query may not be.

*Select query with unique results*

- SELECT DISTINCT column, another_column, …
- FROM mytable
- WHERE condition(s);

### Ordering results

most data in real databases are added in no particular column order. As a result, it can be difficult to read through and understand the results of a query as the size of a table increases to thousands or even millions rows.

SQL provides a way to sort your results by a given column in ascending or descending order using the ORDER BY clause.

*Select query with ordered results*

- SELECT column, another_column, …
- FROM mytable
- WHERE condition(s)
- ORDER BY column ASC/DESC;

"When an ORDER BY clause is specified, each row is sorted alpha-numerically based on the specified column's value. "

### Limiting results to a subset

Another clause which is commonly used with the ORDER BY clause are the LIMIT and OFFSET clauses, which are a useful optimization to indicate to the database the subset of the results you care about. The LIMIT will reduce the number of rows to return, and the optional OFFSET will specify where to begin counting the number rows from.
