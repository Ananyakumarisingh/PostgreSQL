# Queries -
---

__// using smallint, integer, bigint__

Table creation - 

    CREATE TABLE product1(pid serial PRIMARY KEY, pname varchar(100),qty SMALLINT, price integer, sales bigint);

Data Insertion into the Table -

    INSERT INTO product1(pname,qty,price,sales) 
    VALUES ('Sony TV',5,100000,500000),
    ('Alexa',10,8000,80000),
    ('Fire Stick',10,3000,30000);

Get/check the whole table -

    select * from product1;

---

__// using decimal, numeric, real__

Table creation - 

    CREATE TABLE Sales1(sid serial PRIMARY KEY, pname varchar(100), qty SMALLINT, price decimal(10,2), sales numeric(12,2),discount real );

Data Insertion into the Table -

    INSERT INTO Sales1(pname,qty,price,sales,discount) 
    VALUES ('Sony TV',5,100000.00,500000.00,0.10),
    ('Alexa',10,8000.50,80005.50,0.25),
    ('Fire Stick',10,3000.00,30000.00,0.0);

Get/check the whole table -
    
    select * from Sales1;
---

__// create sequence product_id increment by 10 start with 1000 Minvalue 1000 maxvalue 10000;__

Table creation - 

    CREATE TABLE product2(pid smallint default nextval('product_id'), pname varchar(100), qty SMALLINT, price integer, sales bigint);

Data Insertion into the Table -

    INSERT INTO product2(pname,qty,price,sales) 
    VALUES ('Sony TV',5,100000,500000),
    ('Alexa',10,8000,80000),
    ('Fire Stick',10,3000,30000);

Get/check the whole table -
    
    select * from product2;
---

## Enum - 
__// create type product_status as enum('In Stock','Out of Stock','On Sales','Rejected');__

Table creation - 

    CREATE TABLE product3(pid smallint , pname varchar(100), qty SMALLINT, price integer, status product_status);

Data Insertion into the Table -

    INSERT INTO product3(pid, pname, qty, price, status) 
    VALUES (1, 'Sony TV', 5, 10000, 'In Stock'), 
    (2, 'Alexa', 10, 8000, 'In Stock'), 
    (3, 'Fire Stick', 10, 3000, 'On Sales');

Get/check the whole table -
    
    select * from product3;

__// invalid query__

    INSERT INTO product3(pid, pname, qty, price, status) 
    VALUES (4, 'Sony TV', 5, 10000, 'XYZ') 
---


