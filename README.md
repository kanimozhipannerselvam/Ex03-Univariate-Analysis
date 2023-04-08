# Ex03-Univariate-Analysis

Aim

To read the given data and perform the univariate analysis with different types of plots. Explanation

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data. Algorithm

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

PROGRAM

import pandas as pd

import numpy as np

import seaborn as sns

df=pd.read_csv('superstore.csv') df

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

#OUTPUT

![image](https://user-images.githubusercontent.com/119476060/230703771-a57c59cb-8af4-4ce8-861f-086aff069a56.png)

![image](https://user-images.githubusercontent.com/119476060/230703774-999d1e23-dfbb-4155-9bb8-c00953ee0514.png)

![image](https://user-images.githubusercontent.com/119476060/230703779-a2d766af-bf6d-483d-be1b-1206df7f97df.png)

![image](https://user-images.githubusercontent.com/119476060/230703787-fab86a00-b7ca-497a-b7e0-0ba7308021a8.png)

![image](https://user-images.githubusercontent.com/119476060/230703792-7c516ffb-70a8-42ce-97f4-ee68915e39a1.png)

![image](https://user-images.githubusercontent.com/119476060/230703793-adc53bc1-84d1-4d88-ad4e-0e15b0240e6d.png)

![image](https://user-images.githubusercontent.com/119476060/230703795-29b96d98-49d2-457e-881c-c502dbccebde.png)

![image](https://user-images.githubusercontent.com/119476060/230703796-de0dd8ff-6b8a-4fb5-b1ee-5d5d1664bf1a.png)

![image](https://user-images.githubusercontent.com/119476060/230703800-9eebc30d-f0ad-4871-b95f-62c10a5f1fbb.png)

![image](https://user-images.githubusercontent.com/119476060/230703804-da4b0342-e97e-49df-b5d8-1dd140e538bb.png)

![image](https://user-images.githubusercontent.com/119476060/230703808-2bdcd920-263d-46a1-8d53-4848a071bda2.png)

Result

Thus we have read the given data and performed the univariate analysis with different types of plots.











