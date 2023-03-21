# Working with data in python

## Reading&Writing Files with Open

#### Reading

File1 = open("url", [ "w" ])

File1.name

File1.mode

- File1.close()

- with open("url", r"") as <u>File1</u>: (closed outmatically)

  ​        File_content = File1.read()
  
  ![image-20230321230718855](./photo/image-20230321230718855.png)

#### Writing

with open("URL", "W") as F1:
	F1.write("ssss")




## Pandas

Import pandas as pd

df = pandas.read_csv(csv_path)

df = pd.read_excel(excel_path)

Df1.to_csv("path.csv")

**loc selects rows and columns with specific labels**. **iloc selects rows and columns at specific integer positions**

## Numpy in python



