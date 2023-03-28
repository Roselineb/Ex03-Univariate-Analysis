# Ex03-Univariate-Analysis
# Aim:
To read the given data and perform the univariate analysis with different types of plots.
# Explanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
# Algorithm:
# Step1:
Read the given data.
# Step2:
Get the information about the data.

# Step3:
Remove the null values from the data.

# Step4:
Mention the datatypes from the data.

# Step5:
Count the values from the data.

# Step6:
Do plots like boxplots,countplot,distribution plot,histogram plot.
# Program:
NAME: B.ROSELINE

REG: 212221220046

```
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)
```
# Output:
# Dataset:
# ![image](https://user-images.githubusercontent.com/128909895/228205355-4dbba740-92a3-44ee-a573-27dd41ba91a9.png) 
# Head:
# ![image](https://user-images.githubusercontent.com/128909895/228205741-753a07c8-82b5-433e-91a3-5186f21a5e95.png)
# Info:
# ![image](https://user-images.githubusercontent.com/128909895/228206460-ccef85f4-0d1e-4d51-b684-034d40b82795.png)
# Describe:
# ![image](https://user-images.githubusercontent.com/128909895/228206589-2f49ae7d-2b44-4b86-869c-c421fdbf5a85.png)
# Isnull:
# ![image](https://user-images.githubusercontent.com/128909895/228207226-3318cea7-b40c-475a-9fa3-48244c8558cb.png)
# dtypes:
# ![image](https://user-images.githubusercontent.com/128909895/228207790-52e924d0-8c96-4af7-8024-20e8904e6ae6.png)
# Valuecount:
# ![image](https://user-images.githubusercontent.com/128909895/228208356-5ff15a18-c33f-47c0-ac66-0bfe642bd90b.png)
# Boxplot:
# ![image](https://user-images.githubusercontent.com/128909895/228208677-3a6ec632-226f-480e-a05b-e98e3d136006.png)
# Countplot:
# ![image](https://user-images.githubusercontent.com/128909895/228209245-cce27e17-d3ae-4d34-a6f1-4963def4de56.png)
# Distrubution plot:
# ![image](https://user-images.githubusercontent.com/128909895/228209422-0a7b239a-2e29-4024-907d-86c535a5f8de.png)
# Histogram plot:
# ![image](https://user-images.githubusercontent.com/128909895/228210228-ca85efb0-38b0-4ae2-a279-12369ee1ad1d.png)
# Result:
Thus we have read the given data and performed the univariate analysis with different types of plots.



