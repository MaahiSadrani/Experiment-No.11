
# Experiment No. 11: Create and Load Dataset using Pandas
## Aim:
To create a dataset using Python and Pandas, save it as a CSV file, and perform basic data analysis operations. Also, to load an existing dataset and explore its structure and contents.
## Theory:
# Dataset Creation
Dataset- A dataset is a collection of data organized in a structured format such as rows and columns.
In pandas, datasets are represented using a dataframe, which is a 2-dimensional tabular data structure (like an Excel sheet).
Creating Dataset- Creating a dataset means manually defining data inside python and converting it into a dataframe.
A dataset of student details was created using a Python dictionary and converted into a Pandas DataFrame.
Dataset Attributes:
Roll_No
Gender
Department
CGPA
Loading a Dataset- Loading a dataset means importing data from external sources into pandas.
Loading Existing Dataset: An existing dataset (Cars93.csv) was loaded and analyzed.
import pandas as pd
import numpy as np
df = pd.read_csv('/content/Cars93.csv')
import pandas- This line imports the pandas library.Pandas is used for data handling and analysis.
Then a dataset is created through dictionary,list etc.
df = pd.DataFrame(data)-Converts the dictionary into a dataframe and df is now a table.
df.to_csv("students.csv", index=False)-Saves the dataframe into a file named students.csv.
df.shape- It returns the dimensions of the dataframe in the form of (rows,columns).
df.size- It returns the total number of elements (values) in the DataFrame.(size=rows*columns).
df.info() is a function used to get a summary of a dataframe.It gives quick information about the structure of the dataset.It gives number of entries (rows), column names, non-null values, data types and memory usage.
df.describe() is used to generate statistical summary of a dataframe.It mainly works on numerical columns.
count- It gives number of non-null values.
mean- It gives average value.
std-It gives standard deviation (spread of data).
min-It gives minimum value.
25%-It gives first quartile.
0%-It gives median.
75%-It gives third quartile.
max-It gives maximum value.
import numpy as np-It imports NumPy library which is used for numerical operations (arrays, math functions).
df = pd.read_csv('/Cars93.csv')- read_csv() is used to load a dataset from a CSV file and '/Cars93.csv' is the file path.
df.head-It is used to display the first few rows of a dataframe.By default, it shows first 5 rows.
df.tail-It is used to display the last few rows of a dataframe.By default, it shows last 5 rows.
df.sample(5) is used to select random rows from a dataframe.It returns 5 random rows from the dataset.
df.columns is used to get the names of all columns in a dataframe.
df.isnull().sum()-It is used to check missing (null) values in each column of a datarfame.
df.duplicated().sum()-It is used to find the number of duplicate rows in a dataframe.
df.nunique() is used to count the number of unique (distinct) values in each column of a dataframe.
Conclusion:
This experiment demonstrated how to create a dataset in Python using Pandas, save it as a CSV file, and load external datasets for analysis.
It also helped in understanding basic DataF


## Conclusion:
Therefore we learn
* How to create and save datasets using Pandas
* How to load external datasets
* Performing exploratory data analysis (EDA)
* Identifying missing values and dataset structure
using python
Pandas provides powerful and efficient tools for handling structured data in Python.
## Refrence Images:

<img width="1120" height="783" alt="Screenshot 2026-03-30 105455" src="https://github.com/user-attachments/assets/18fe136b-f57e-4bb0-b91b-6ecb681eb4cd" />
<img width="1119" height="786" alt="Screenshot 2026-03-30 105422" src="https://github.com/user-attachments/assets/83549fcb-2867-4019-a3c3-33249fa03091" />
<img width="1117" height="791" alt="Screenshot 2026-03-30 105343" src="https://github.com/user-attachments/assets/0583198c-d804-4594-bffd-3f7d5a451c7c" />
