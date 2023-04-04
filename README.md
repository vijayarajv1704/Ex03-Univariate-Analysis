# Ex03-Univariate-Analysis

Aim

To read the given data and perform the univariate analysis with different types of plots.
Explanation

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
Algorithm

Step1

Read the given data.

Step2

Get the information about the data.

Step3

Remove the null values from the data.

Step4

Mention the datatypes from the data.

Step5

Count the values from the data.

Step6

Do plots like boxplots,countplot,distribution plot,histogram plot.

Program

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

OUTPUT

![image](https://user-images.githubusercontent.com/121303741/229699516-7c113f9a-9577-4557-9544-9c3841672e09.png)


![image](https://user-images.githubusercontent.com/121303741/229699537-3d776992-5ae8-4412-9e66-0f8a6de1fe3b.png)

![image](https://user-images.githubusercontent.com/121303741/229699570-5ef8383f-b47f-43da-9dc6-a371b4258612.png)

![image](https://user-images.githubusercontent.com/121303741/229699596-7cd9617f-d2af-4ebb-8c17-ea64d932b2c4.png)

![image](https://user-images.githubusercontent.com/121303741/229699625-3be7f222-65b3-4c52-8f45-c0b8272a8216.png)

![image](https://user-images.githubusercontent.com/121303741/229699657-982b24c3-7ada-4cc0-af81-a220afd5c317.png)

![image](https://user-images.githubusercontent.com/121303741/229699640-7baa1694-34e6-48ab-89ad-014bdf764eed.png)

![image](https://user-images.githubusercontent.com/121303741/229699670-98065a7c-c0b2-49d1-b47f-d2400c99d6d1.png)

![image](https://user-images.githubusercontent.com/121303741/229699700-6545973b-7b22-4910-8b9b-ebcaaa7883c6.png)

![image](https://user-images.githubusercontent.com/121303741/229699711-de4e04b1-d44d-430b-963d-39cd7aed4b7d.png)

![image](https://user-images.githubusercontent.com/121303741/229699773-c95a9165-10b8-414f-bfbd-ee41f16427c8.png)

![image](https://user-images.githubusercontent.com/121303741/229699791-ed8a7ad1-a5d5-4c20-a2a1-29548963e490.png)

Result

Thus we have read the given data and performed the univariate analysis with different types of plots.

