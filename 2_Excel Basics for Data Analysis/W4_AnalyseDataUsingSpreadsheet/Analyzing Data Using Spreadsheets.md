# Analyzing Data Using Spreadsheets

##### Learning Objectives
- Describe the fundamentals of analyzing data using a spreadsheet
- **Filter** and **sort** data in a worksheet.
- Employ some of the most useful Excel functions for data analysis.
- Implement the VLOOKUP and HLOOKUP functions to reference data.
- Create **pivot** tables in Excel.
- Utilize pivot table features.

## Data Analysis Basics, Diltering and Sorting Data

### Intro to Analyzing Data Using Spreadsheets

What should be considered before changes maken:	

(1)How big is the dataset

(2)What type of filtering is required to find the necessary information

(3)How should the data be sorted

(4)what type of calculations are needs

------

- 1Filtering

- 2Sorting

  Alphabetically, numerically

- 3Performing Calculations

  Excel: Mathematical, Statistical, Logical, Financial, Data and Time

- 4Shaping out data

### Filtering and Sorting Data in Excel

##### Filtering

##### Ordering

- Text-based data - Alphabetically
- Number-based data - Numerically
- Data-based data - Chronologically

### Useful Functions for Data Analysis

- IF

  =IF(AD2>300,"Large",IF(AD2>100,"Medium",IF(AD2>0,"Small")))

- IFs: nested IF function

  =IFS(AD3>300,"Large",AD3>100,"Medium",AD3>0,"Small")

- Conditional Formatting

- CountIF

- SUMIF; SUMIFS

  =SUMIF(range, criteria, [sum range])

### Using VLOOKUP and HLOOKUP Functions

B3: the value i am looking for

![image-20230309163313211](./photo/image-20230309163313211.png)

=VLOOKUP (value, table, col_index, [range_lookup])

Advanced vhlookup method: https://www.zhihu.com/question/27224727



| VLOOKUP | (value, table_array,col_index,range) |
| -------- | -------|
| value | use "which one" to find |
| Table_array |where to find|
| Col_index |which col will be return|
| Range |exact or approximate|
| **Multiple layer** |  |
| COLUMN |COLUMN() the order must  be mactched with original tale; the value we what to find must lay among the first col<br />VLOOKUP($L12, $A$4:$J$21, COLUMN(G4),0)|
| Match |VLOOKUP($L12, $A$4:$J$21, MATCH(M$18, $A$3,),0)|
|  ||
| VLOOKUP |reverse lookup|
| XLOOKUP |reverse lookup|
| VLOOKUP |double search|
| XLOOKUP |double search|
| one to more lookup ||









