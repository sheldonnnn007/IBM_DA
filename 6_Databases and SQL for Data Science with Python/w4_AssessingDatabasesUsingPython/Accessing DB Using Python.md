# Accessing DB Using Python

## How to Access Databases Using Python

<img src="./photos/image-20230330102347571.png" alt="image-20230330102347571" style="zoom:50%;" />

## Writing code using DB-API

Program open a "Connection" to gain it's contents
A "cursor" is like a file handle to have access to query

![image-20230330104650390](./photos/image-20230330104650390.png)

##### Connection methods

.cursor()
.commit()
.rollback()
.close()

##### Cursor method:

.callpro()
.execute()
.executemany()
.fetchone()
.fetchmany()
.fetchall()
.nextset()
.arrysize()
.close()

## Connecting to a databse using ibm_db API

<img src="./photos/image-20230330105623205.png" alt="image-20230330105623205" style="zoom:50%;" />

<img src="./photos/image-20230330105709789.png" alt="image-20230330105709789" style="zoom:50%;" />

CLOSE: ibm_db.close(conn)



## Creating tables, loading data and querying data

stmt = Ibm_db.exec_immediate(conn)<img src="./photos/image-20230330111446075.png" alt="image-20230330111446075" style="zoom:50%;" />

Query:
Ibm_db.fetch_both(stmt)

##### Using Pandas

<img src="./photos/image-20230330111903296.png" alt="image-20230330111903296" style="zoom:50%;" />





## Analyzing data with python

stmt = ibm_db.exec_immediate(conn,"SELECT count(*) FROM MC")
Ibm_db.fetch_both(stmt)

pconn = ibm_db_dbi.Connection(***conn***)
df = pandas.read_sql("Command", pconn)
df





Magic SQL:

<img src="./photos/image-20230330232336806.png" alt="image-20230330232336806" style="zoom:50%;" />

<u>%%sql</u>: the whole cell is sql command

###### Using Python Variables in your SQL Statements
country = "Canada"
<u>%sql</u> select * from INTERNATIONAL_STUDENT_TEST_SCORES where country = :country

###### Assigning the Results of Queries to Python Variables

<img src="./photos/image-20230330234506617.png" alt="image-20230330234506617" style="zoom:50%;" />
dataframe = test_score_distribution.DataFrame().   can change result to DataFrame directly

W4:https://www.coursera.org/learn/sql-data-science/ungradedLti/GUr2q/optional-hands-on-lab-analyzing-a-real-world-data-set



