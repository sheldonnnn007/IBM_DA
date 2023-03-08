# Basics of Data Quality and Privacy

(Garbage in Garbage out)

 #### 5 Traits of Good Data

- Accuracy
- Completeness
- Timeliness
- Reliability
- Relevance

#### Importing File Data

- How to import: Data Import Wizard
- How to adjust column widths
- How to add and remove columns and rows

#### Basics of Data Privacy
##### Confidentiality
- PI(Personal Information): information that can be traced back to a specific individual.
- PII(Personal Identifiable Information): info could be used to identify an individual. (social security number or driver's license number
- SPI(Sensitive Personal Information): contains private info that needs to be protected (race, sexual orientation, biometrics, genetic information
##### Collection and Use

When searching through data, the analyst must know the location of the company collecting the data and the location of the respondent. (Knowing what regulations must be applied)

Hefty fines

##### Compliance

remain compliant when we handle infos





# Cleaning Data

### Removing Duplicated or Inaccurate Data and Empty Rows

- How to deal with inaccurate data
- How to remove empty rows
- How to remove duplicated data

### Dealing with Inconsistencies in Data

- How to change the case of text

  Change case

- How to change data formatting

- How to <u>trim</u> whitespace from data

### More Excel Features for Cleaning Data

- Flash Fill
  Naming Convention
- Text to Columns





## Hands-on lab

After completing this lab, you will be able to:

- Understand how to deal with irrelevant or inaccurate data
- Remove empty rows and duplicated data
- Change text case and date formatting
- Trim whitespaces from data
- Use Flash Fill and functions to clean data

In cell **A2** type **=LEFT(C2, SEARCH(“ “,C2,1))** and press **Enter**.

In cell **B2** type **=RIGHT(C2,LEN(C2)-SEARCH(“ “,C2,1))** and press **Enter**.
