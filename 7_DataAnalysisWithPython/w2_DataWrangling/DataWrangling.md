# DataWrangling

## Pre-processing Data in python

(Data Cleaning; Data Wrangling)



## Dealing with Missing Values in Python

<img src="./photos/image-20230402214139096.png" alt="image-20230402214139096" style="zoom:50%;" />

## Dealing with Missing Values in Python

<img src="./photos/image-20230402220115641.png" alt="image-20230402220115641" style="zoom:50%;" />

- <u>Drop</u>: Df.fropna() use axis = 0,1 to denote to delete row0 or column1

<img src="./photos/image-20230402220749463.png" alt="image-20230402220749463" style="zoom:50%;" />

- <u>Replace</u>: df.replace(missing_calue, new_values)

## Data Formatting in Python

<img src="./photos/image-20230402221520187.png" alt="image-20230402221520187" style="zoom:50%;" />

<img src="./photos/image-20230402222123849.png" alt="image-20230402222123849" style="zoom:50%;" />

## Data Normalization in Python

The different **range**s of different features will influence the future analysis such as regression. SO WE NEED NORMALIZATION

##### 3 ways

<img src="./photos/image-20230402223701890.png" alt="image-20230402223701890" style="zoom:50%;" />
3⃣️deviation sigma; and the resulting values hover around zero, typically range -3 and 3(but can be higher or lower)

- Z-score 

<img src="./photos/image-20230402224726088.png" alt="image-20230402224726088" style="zoom:50%;" />



## Binning in Python

<img src="./photos/image-20230402225143358.png" alt="image-20230402225143358" style="zoom:50%;" />

bins = np.linspace(min(df["price"]), max(df["price"]), 4)
Group_name = ["Low", "Medium", "High"]
Df["price-binned"] = pd.<u>cut</u>(**df["price"]**, bins, labels = group_name, include_lowest = True)

## Turning categorical variables into quantitative variables

##### Problem: Most statistical models cannot take in the objects/strings as input. ( One-Hot )

<img src="./photos/image-20230402230557187.png" alt="image-20230402230557187" style="zoom:50%;" />

- get_dummies()

  pd.get_dummies(df['fuel']): automatically generates a list of numbers each one corresponding to a particular category of the variable.