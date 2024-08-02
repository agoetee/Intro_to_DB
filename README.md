# About  Introductions to Databases

## 0. A Magical Database for Your Dream Online Bookstore Adventure! 

Imagine you’re tasked with designing a MySQL database for an online bookstore. The database should store information about books, authors, customers, orders, and order details. Here’s an overview of the database schema:

Database Name: `alx_book_store`

 - Books: Stores information about books available in the bookstore.
    - book_id (Primary Key)
    - title VARCHAR(130)
    - author_id (Foreign Key referencing Authors table)
    - price DOUBLE
    - publication_date DATE

 - Authors: Stores information about authors.
    - author_id (Primary Key)
    - author_name VARCHAR(215)

 - Customers: Stores information about customers.
    - customer_id (Primary Key)
    - customer_name VARCHAR(215)
    - email VARCHAR(215)
    - address TEXT

 - Orders: Stores information about orders placed by customers.
    - order_id (Primary Key)
    - customer_id (Foreign Key referencing Customers table)
    - order_date DATE

- Order_Details: Stores information about the books included in each order.
    - orderdetailid (Primary Key)
    - order_id (Foreign Key referencing Orders table)
    - book_id (Foreign Key referencing Books table)
    - quantity DOUBLE

NOTE : - The file extension should be `alx_book_store.sql` file - All SQL keywords should be in uppercase

__Repo:__

- GitHub repository: `Intro_to_DB`
- File: `alx_book_store.sql`


## 1. Let's Build Your Database: Your Gateway to Data Adventure! 

Write a simple python script that creates the database `alx_book_store` in your MySQL server.

- Name of python script should be `MySQLServer.py`
- If the database `alx_book_store` already exists, your script should not fail
- You are not allowed to use the `SELECT` or `SHOW` statements

NOTE :

- Required to print message such as Database `'alx_book_store' created successfully!` when database is successfully created.

- Print error message to handle errors when failing to connect to the DB.

- handle open and close of the DB in your script.

__Repo:__

- GitHub repository: `Intro_to_DB`
- File: `MySQLServer.py`



