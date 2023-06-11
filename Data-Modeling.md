# Data Modeling

## NoSQL vs SQL

1. What type of database is the best fit for the complex query intensive environment?

**SQL** databases are suitable for complex query-intensive environments. They use SQL (structured query language) to define and manipulate data, which is powerful. In contrast, **NoSQL** databases are not suitable for complex queries. On a high level, NoSQL does not have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as the SQL query language.

2. What type of database is the best fit for hierarchical data storage?

NoSQL databases are better suited for hierarchical data storage as they follow the key-value pair way of storing data similar to JSON data. SQL databases are not the best fit for hierarchical data storage.

3. The differences in scalability between a SQl and NoSQL database

SQL databases are vertically scalable which means that you can manage increasing load by increasing the CPU, RAM, SSD, etc., on a single server. On the other hand, NoSQL databases are horizontally scalable which means that you can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.

In simple words, SQL databases are like a single-story house that you can make bigger by adding more rooms or making the existing rooms bigger. NoSQL databases are like a multi-story building that you can make bigger by adding more floors.

## SQL Modeling Techniques

1. Among data tables, what is a one-to-many relationship and how do we “relate” them?

**one-to-many** relationship is when an entry in one table can be related to more than one entry in another. For example, there are many employees in one department. We show this relationship by connecting lines between tables showing that we have a one-to-many relationship. 

2. Prior to designing your relational database, it might be useful to ___ a ___ of the database tables and their relationships.

Before designing the relational database, it might be useful to create a **diagram** of the database tables and their relationships. These may be done during the design process, as the data modeling, or once the database is created, in order to document the tables’ dependencies. 

3.  the difference between a primary and foreign key.

A **primary key** is a column or set of columns that uniquely identify each row in a table. A table typically has one primary key but can have more. When the key has more than one column, it is called a compound key. A **foreign key** is a column or set of columns that match a primary key in another table. The match between foreign keys and primary keys is what “glues” the database together and makes a relationship between them. 

## SQL vs NoSQL

1. How do we treat keywords and parameters differently in SQL syntax?

In SQL syntax, **keywords** are reserved words that have a specific meaning in the language. They are used to define the structure of the query and cannot be used as identifiers such as table or column names. **Parameters** are values that are passed to a query at runtime. They are used to filter data or define the behavior of the query.

2. Define normalization within the context of schemas and data.

**Normalization** is a process of organizing data in a database. It involves creating tables and establishing relationships between them to reduce redundancy and improve data integrity. Normalization is usually done in stages called normal forms. The most common normal forms are the first normal form (1NF), second normal form (2NF), and third normal form (3NF).

3.  the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.

In the context of schemas and data, **one-to-one** relationship is when an entry in one table can be related to only one entry in another table. **One-to-many** relationship is when an entry in one table can be related to more than one entry in another table. **Many-to-many** relationship is when entries in both tables can be related to multiple entries in each other.