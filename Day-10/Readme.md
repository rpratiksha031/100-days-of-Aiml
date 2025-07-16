# 📊 Day 10 of 100 Days of AI/ML — Mastering pandas: Series, DataFrames & Core Operations

Today’s focus was diving deeper into **pandas**, the Python library at the heart of data analysis and preprocessing.  
I explored its two primary data structures — **Series** and **DataFrames**, and learned the most common and useful operations on them.

---


Series : It is one dimensional labeled array holding data of any type 
import pandas as pd

s = pd.Series([10, 20, 30, 40])
print(s)

0    10
1    20
2    30
3    40
dtype: int64




Dastaframe: It two dimensional array holding data of any type with rows and columns .

data = {
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Age': [25, 30, 35]
}
df = pd.DataFrame(data)
print(df)


      Name  Age
0    Alice   25
1      Bob   30
2  Charlie   35


what are the main things we are gonna learn here :
> Object creation 
>Viewing data 
>Selection 
>Missing data 
>Operations 


### 1. Object creation: 
 Creating Series and DataFrames from various data types:
s = pd.Series([1, 2, 3])
df = pd.DataFrame([[1, 2], [3, 4]], columns=['A', 'B'])

From Dictionaries:
data = {'a': 10, 'b': 20}
s = pd.Series(data)

data = {'Name': ['Tom', 'Jerry'], 'Score': [85, 92]}
df = pd.DataFrame(data)


### 2. Viewing Data
To understand the structure or content of your data:
df.head()         # First 5 rows
df.tail()         # Last 5 rows
df.shape          # (rows, columns)
df.columns        # Column names
df.index          # Row indices
df.info()         # Summary
df.describe()     # Statistical summary (numerical only)

### 3. Selection (Indexing & Filtering)
Selecting Columns:
df['Name']          # Single column (Series)
df[['Name', 'Age']] # Multiple columns (DataFrame)

Selecting Rows:
df.loc[0]       # Row by label
df.iloc[0]      # Row by position

Filtering Data:

df[df['Age'] > 30]


### 4. Handling Missing Data
 Creating Missing Data:
  import numpy as np
df = pd.DataFrame({
    'A': [1, np.nan, 3],
    'B': [4, 5, np.nan]
})

Detecting Missing Data:
 df.isnull()
df.notnull()
 
Removing Missing Data:
df.dropna()  # Drop rows with any NaN values

Filling Missing Data:
df.fillna(0)  # Replace NaN with 0
df.fillna(df.mean())  # Replace NaN with column mean

### 5. Operations on Data

Basic Arithmetic:
df['A'] + df['B']

Statistical:
df.mean()
df.sum()
df.max()
df.min()
df.count()

Apply a Function:
df['A'].apply(np.sqrt)
df['Name'].apply(len)

Sorting:
df.sort_values(by='Age')
df.sort_index()

Rename Columns:
df.rename(columns={'Name': 'FullName'})



















