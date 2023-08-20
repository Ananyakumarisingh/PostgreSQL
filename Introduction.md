# PostgreSQL

### Lists various database management systems (DBMS) or database software that are commonly used for managing and storing data.

1. MS SQL SERVER
2. MySQL
3. Oracle
4. MongoDB
5. PostgreSQL
---
### Types of Databases:

1. __Centralized Database__ - Stores data like employee details, customer details in a single location.
2. __Distributed Database__ - Spreads data across multiple servers or locations.
3. __Personal Database__ - Used for personal purposes like WhatsApp chats.
4. __End-User Database__ - Holds data from individual users, like fitness tracking details or a personal movie collection.
5. __Commercial Database__ - Used by large platforms like Amazon and Flipkart.
6. __No-SQL Database__ - Example: MongoDB, which stores data in JSON-like documents.
7. __Object-Oriented Database__ - Example: PostgreSQL, which can handle object-oriented and relational data.
8. __Relational Database__ - Utilizes primary keys and foreign keys to establish relationships between tables.
---
### What is PostgreSQL?

- It's an open-source database management system.
- It's both an object-oriented and relational database.
- It supports both SQL (relational) querying and JSON (non-relational) querying.
---
### Who uses PostgreSQL?

> Companies such as __Uber__, __Instagram__, __Spotify__, __Skype,__ and __Cisco__ utilize PostgreSQL for their database needs.

---
### MongoDB

- MongoDB is a type of database that is schema-free, meaning it can handle data in JSON format without requiring a strict structure.
- It uses the concept of collections to store data instead of tables in a traditional relational database.
- Data is stored in documents, which are similar to JSON objects.
- MongoDB is a non-relational database.
- It uses indexes to optimize query performance.
- It's designed with a distributed architecture in mind.
---
### PostgreSQL

- PostgreSQL is SQL-based but also supports NoSQL features.
- It's a relational database that uses the concept of tables to store data.
- It supports joins to combine data from different tables.
- It's designed using a monolithic architecture.
- PostgreSQL offers a wide range of predefined functions compared to other databases like MS SQL Server or MySQL.
---
### PostgreSQL Features

- User-defined Datatypes
- Table Inheritance
- Foreign Keys
- Views, Rules, Subqueries
- Nested Transactions

---
### Languages used with PostgreSQL

- Functions and procedures can be written using __Python__.
---
### List of Datatypes

1. Numeric
    1. smallint 	- 2 bytes	-	(-32768 to +32767)
    2. integer	- 4 bytes	-
    3. bigint	- 8 bytes	- 	
    4. decimal	- variable 	- 	upto 131072 (digits before and after a decimal point) .
    5. numeric	- upto 131072 (digits before and after a decima 1 point 16383) .
    6. real		- 4 byte
    7. serial	- 4 bytes (auto increment)
    8. smallserial  - 2 bytes
    9. bigserial	- 8 bytes
2. Monetary
3. Character
4. Binary
5. Date/Time
6. Boolean
7. Enumerated 
8. Network Address
9. Range Type
10. Bit String
11. Text Search
12. UUID
13. XML
14. JSON
15. Geometric
16. Arrays
17. Composite
18. Domain
19. Object identifier
20. pseudo


### Difference between Sequence and Serial
| Sequence | Serial |
|---|---|
| - sequence are not available in all db mgmt system. | - sequence are not available in all db mgmt system.
| - PostgreSQl, Orcle, MS SQL Server. | - PostgreSQl, Orcle, MS SQL Server.
| - Create Sequence statement | - Create Sequence statement
---

### Auto increment

- Available in all db mgmt system
- autoincrement is part of table's schema.
- in MySQL (autoincrement) - can use only autoincrement.
- in MS SQL Server (identity(1,1))
---

### Enum ( from c programming enum )
- can give some constant values.
- enum is a special datatype
- It allows to define a list of possible values for a column.
---

