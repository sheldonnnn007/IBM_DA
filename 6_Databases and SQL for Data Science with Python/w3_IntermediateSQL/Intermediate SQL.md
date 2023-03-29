# Intermediate SQL

## Refining your result

### Using <u>String Patterns</u> and Ranges

- Like: WHERE first name LIKE R%

  % persent sign is used to define the missing letters; which can be placed b<u>efore/after/b and a</u> the pattern

- between .. and .. (instead of AND)

  <img src="./photos/image-20230329110751550.png" alt="image-20230329110751550" style="zoom:50%;" />

- IN (instead of OR)

  <img src="./photos/image-20230329111002675.png" alt="image-20230329111002675" style="zoom:50%;" />

  

### <u>Sorting</u> Result Sets

how to indicate which column to use for the sorting order
(Alphabetical order)

###### ORDER BY
ascending order by default

<img src="./photos/image-20230329111521231.png" alt="image-20230329111521231" style="zoom:50%;" />

Is the start letter same, so the sorting will be started from the point where the characters differ.

Use number to indicate the column
select title, page from Book <u>ORDER BY 2</u>;



### <u>Grouping</u> Result Sets

I want to know which country the authors from and how many authors come  from each country.

<img src="./photos/image-20230329112345859.png" alt="image-20230329112345859" style="zoom:50%;" />

<img src="./photos/image-20230329112507674.png" alt="image-20230329112507674" style="zoom:50%;" />

###### Having ("where" clause is for the entire result set, "Having" works only with group by )

<img src="./photos/image-20230329112742605.png" alt="image-20230329112742605" style="zoom:50%;" />





## Functions, Multiple Tables, ans Sub-queries

### Built-in Database Functions

Can speed up data processing: rather than first retriving the data onto your application and then process

###### Aggregate function: SUM(), MIN(), MAX(), AVG()

<img src="./photos/image-20230329114059063.png" alt="image-20230329114059063" style="zoom:50%;" />

###### Give Alias:

select SUM(COST as SUM_OF_COST from PETRESCURE

<img src="./photos/image-20230329114647532.png" alt="image-20230329114647532" style="zoom:50%;" />

##### Scalar and String Functions

Round(), Length(), Ucase, Lcase,

<img src="./photos/image-20230329115012834.png" alt="image-20230329115012834" style="zoom:50%;" />

<img src="./photos/image-20230329115314192.png" alt="image-20230329115314192" style="zoom:50%;" />

<img src="./photos/image-20230329115417902.png" alt="image-20230329115417902" style="zoom:50%;" />

If i do not clear about the Upper or Lower case used in cells when I use WHERE, i can use <u>UCASE and LCASE</u>

### Data and Time Built-in Functions

<img src="./photos/image-20230329115757579.png" alt="image-20230329115757579" style="zoom:50%;" />

###### Functions: YEAR(), MONTH(), DAY(), DAYOFMONTH(), DAYOFWEEK(), DAYOFYEAR(), WEEK(), HOUR(), MINUTE(), SECOND()

Select DAY(data_column)
Select (data_column + 3 <u>DAYS</u>) from table

- special registers: **CURRENT_DATE, CURRENT_TIME**

  Select (CURRENT_DATE - data_column) from table

can conbine with WHERE clause as well



### Sub_Queries and Nested Selects

Sub_Q is like a regular query but placed within parentheses and nested inside another query

<img src="./photos/image-20230329121120639.png" alt="image-20230329121120639" style="zoom:50%;" />





##### Utilized with WHERE
<u>The limitation of aggregate function:</u>
<img src="./photos/image-20230329121402503.png" alt="image-20230329121402503" style="zoom:50%;" />

how to circumvent this limitation: Nested query<img src="./photos/image-20230329121626237.png" alt="image-20230329121626237" style="zoom:50%;" />

#### Other utilisations

<img src="./photos/image-20230329122002165.png" alt="image-20230329122002165" style="zoom:50%;" />

<img src="./photos/image-20230329122200298.png" alt="image-20230329122200298" style="zoom:50%;" />





### Working with ***multiple*** Tables

1. Sub_queries

<img src="./photos/image-20230329122614399.png" alt="image-20230329122614399" style="zoom:50%;" />

<img src="./photos/image-20230329122830028.png" alt="image-20230329122830028" style="zoom:50%;" />

<img src="./photos/image-20230329123132516.png" alt="image-20230329123132516" style="zoom:50%;" />





2. Implicit JOIN

<img src="./photos/image-20230329123525760.png" alt="image-20230329123525760" style="zoom:50%;" />

<img src="./photos/image-20230329124045972.png" alt="image-20230329124045972" style="zoom:50%;" />

BTW the result table columns will be like :  E.column_name

<img src="./photos/image-20230329124356381.png" alt="image-20230329124356381" style="zoom:50%;" />

<img src="./photos/image-20230329124458413.png" alt="image-20230329124458413" style="zoom:50%;" />









