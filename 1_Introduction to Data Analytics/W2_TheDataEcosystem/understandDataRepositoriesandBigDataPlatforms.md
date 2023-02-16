# Overview of Data Repositories

### Databases

#### Factors governing choice of database include:

- Data type
- Data structure
- Querying mechanism
- Latency requirements
- Transaction speeds
- Intended use of data

#### Relational(RDBS) and Non-relational databases

- Relational Databases(Relational Database Managent System RDBMS): A relational database is a collection of data organized into a table structure, where the tables can be linked, or related, based on data common to each.

- Advantages:
  
  Creating meaningful information by joining tables;
  
  Flexibility to make changes while the database is in use;
  
  Minimize data redundancy by allowing relationships to be defined between tables.
  
  Ease of backup and disaster recovery 
  
  ACID compliant: Atomicity, Consistency, Isolation, Durability
  
- Use Cases for RDBMS

  Online Transaction Processing (OLTP)

  Data Warehouse

  IoT Solutions
  
- Limitation of RDBMS

  Does not work well with semi-structured and unstructured data 

  Migration between to RBDMs is possible only when souce and destination table hace identical schemas and data types

  Entering a value greater than the defined length of a data field results in loss information.

  

