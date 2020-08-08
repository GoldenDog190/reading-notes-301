# Online Readings

## [Complete SQLBolt (Intro, Lessons 1-4, 13-18)](http://sqlbolt.com/)
**Introduction to SQL**
* SQL(Structured Query Language) - is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. 
* Relational database - represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.
* SQL goal is to learn how to answer specific questions about data, and make better decisions about it.

* SQL Lesson 1: SELECT queries 101
  - To retrieve data from a SQL database, we need to write SELECT statements, which are refered to as queries. A query is just a statement which declares what data we are looking for, where to find it in the database, and how to transform it before it is returned. 
  - Table in SQL is a type of entity.
  - Columns represent the common properties shared by all instances of that entity.
  - The most basic query we could write would be one that selects for a couple columns (properties) of the table with all the rows (instances). 
  - Exercise 1 Task Answers:
    1. SELECT title FROM movies;
    2. SELECT director FROM movies; 
    3. SELECT title, director FROM movies;
    4. SELECT title, year FROM movies;
    5. SELECT * FROM movies;

* SQL Lesson 2: Queries with constraints (Pt. 1)
  - WHERE clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not. More complex clauses can be constructed by joining numerous AND or OR logical keywords. 
  - Write SQL keywords all capitalized.
  - Exercise 2 Task Answers:
    1. SELECT id, title FROM movies 
       WHERE id = 6;
    2. SELECT title, year FROM movies
       WHERE year BETWEEN 2000 AND 2010;
    3. SELECT title, year FROM movies
       WHERE year NOT BETWEEN 2000 AND 2010; 
    4. SELECT title, year FROM movies
       WHERE year <= 2003;

* SQL Lesson 3: Queries with constraints (Pt. 2)
  - When writing WHERE clauses with columns containing text data, SQL supports a number of useful operators to do things like case-insensitive string comparison and wildcard pattern matching.
  - All strings must be quoted so that the query parser can distinguish words in the string from SQL keywords.
    - Exercise 3 Task Answers:
    1. SELECT title, director FROM movies 
       WHERE title LIKE "Toy Story%";
    2. SELECT title, director FROM movies 
       WHERE director = "John Lasseter";
    3. SELECT title, director FROM movies 
       WHERE director != "John Lasseter"; 
    4. SELECT * FROM movies 
       WHERE title LIKE "WALL-_";

* SQL Lesson 4: Filtering and sorting Query results
  - DISTINCT keyword - way to discard rows that have a duplicate column value.
  - GROUP BY clause - discard duplicates based on specific columns using grouping.
  - ORDER BY clause - provides a way to sort your results by a given column in ascending or descending order. When specified, each row is sorted alpha-numerically based on the specified column's value.
  - LIMIT and OFFSET clauses - LIMIT will reduce the number of rows to return, and OFFSET will specify where to begin counting the number rows from. Applied last.
     - Exercise 4 Task Answers:
    1. SELECT DISTINCT director FROM movies
       ORDER BY director ASC;
    2. SELECT title, year FROM movies
       ORDER BY year DESC
       LIMIT 4; 
    3. SELECT title FROM movies
       ORDER BY title ASC
       LIMIT 5;
    4. SELECT title FROM movies
       ORDER BY title ASC
       LIMIT 5 OFFSET 5;
       
* SQL Lesson 13: Inserting rows
  - 



## [W3 Schools](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all)


# Additional Resources
## [A Primer on SQL](https://openlibra.com/en/book/a-primer-on-sql-3rd-edition)

**Introduction to SQL(Structured Query Language)**
* 

## [SQL Cheat Sheet](http://www.cheat-sheets.org/sites/sql.su/)

**SQL Cheat Sheet**

* A quick cheat sheet for SQL(Structured Query Language) on one page.
* Includes:
  - Database Manipulation
  - Table Manipulation
  - Index Manipulation
  - Data Manipulation
  - Select
  - Alias
  - Join
  - Union
  - Select into/in 
  - Create view