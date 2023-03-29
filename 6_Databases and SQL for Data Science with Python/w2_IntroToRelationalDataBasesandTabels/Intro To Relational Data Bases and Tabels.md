# Intro To Relational Data Bases and Tabels

### ERD

Entity-Relationship Model
<img src="./photos/image-20230328111821320.png" alt="image-20230328111821320" style="zoom:50%;" />
Primary key of a relational table uniquely identifies each tuple or row in a table, preventing duplication.
Foreign keys which are primary keys defined in orther tables, creating a link between two tables.

### Cloud Databases

Which can Expand/Shrink(accommodate changing needs and usage demands) Storage & Compute Resources
Pay per use

##### Database as Service DBaaS

DBaas provide users with access to Database resources in cloud without setting up underlying hardware and installing software.

## Type of SQL statements (DDL vs DML)

SQL statements fall into two diff categories: 

<img src="./photos/image-20230328115611818.png" alt="image-20230328115611818" style="zoom:50%;" />

- **Data Definition Language**: <u>Define, Change, or drop data</u>

  Create, 

  Alter(adding and dropping columns and modify their data types), 

  Truncate(delating data in the table but not table itself) 

  and drop(deleting tables)

- **Data Manipulation Language**: 

  Read and modify data

  CRUD operations(Create, Read, Update, Delete)

  INSERT

  SELECT

  UPDATE

  DELETE

## CREATE TABLE Statement

![image-20230328120754335](./photos/image-20230328120754335.png)

Primary key not null: This **constraint** prevents duplicate values in the table

Names of columns; Datatypes of columns; Constraints (e.g. Primary Key)

## <u>Alter</u>, Drop and Truncate 



<img src="./photos/image-20230328121621163.png" alt="image-20230328121621163" style="zoom:50%;" />

<img src="./photos/image-20230328121842841.png" alt="image-20230328121842841" style="zoom:50%;" />

BIGINT can hold a number up to 19 digits long

![image-20230328122429971](./photos/image-20230328122429971.png)
Values in cells must compatiable with new type



delete the table , not only data
![image-20230328122907530](./photos/image-20230328122907530.png)



<img src="./photos/image-20230328122700993.png" alt="image-20230328122700993" style="zoom:50%;" />



<img src="./photos/image-20230328123108288.png" alt="image-20230328123108288" style="zoom:50%;" />



