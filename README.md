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
# Ex03-Univariate-Analysis

# CODE:

```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv("SuperStore.csv")
print(df)
df.head()
df.info()
df.dtypes
df.describe()
sns.boxplot(x='Postal Code',data=df)
sns.countplot(x="Postal Code",data=df)
sns.histplot(x="Postal Code",data=df)
df.skew()
sns.boxplot(x="Sales",data=df)
sns.histplot(x='Postal Code',data=df)
sns.displot(x="Postal Code",data=df)
df.kurtosis()
sns.boxplot(x="Sales",data=df)
```
```
import pandas as pd
import seaborn as sns
df1=pd.read_csv("diabetes.csv")
print(df1)
df1.info()
df1.dtypes
df1.skew()
df1.describe()
sns.boxplot(x='Glucose',data=df1)
sns.countplot(x="Glucose",data=df1)
sns.displot(df1["Glucose"]) 
sns.histplot(x="Glucose",data=df1)
df1.skew()
df1.kurtosis()
sns.boxplot(x="Insulin",data=df1)
```

# Output:

![df data](https://user-images.githubusercontent.com/114852180/227990250-b6352791-6a17-447f-94f3-6dc0daec22c9.png)
![df info](https://user-images.githubusercontent.com/114852180/227991011-ec331ff4-a41a-47fd-b7b0-d015ad4a33c0.png)
![df datatypes](https://user-images.githubusercontent.com/114852180/227991623-9b1e712c-2f4c-4c44-a977-94156481e980.png)
![df describe](https://user-images.githubusercontent.com/114852180/227992293-00eb2139-ebf5-4b86-8547-045a970f73a3.png)
![df boxplot](https://user-images.githubusercontent.com/114852180/227992458-a1e17460-5a49-4fb5-b08a-a5f8b96e26eb.png)
![df histplot](https://user-images.githubusercontent.com/114852180/227992690-29d431b9-3ea5-4cd2-b89d-6c7ca83c141a.png)
![df skew](https://user-images.githubusercontent.com/114852180/227993433-caec0b70-8bac-41e7-a577-0e58b0e366b2.png)
![df count plot](https://user-images.githubusercontent.com/114852180/227995969-b72c37a5-fdca-44e5-8768-c15bc6495fef.png)
![df kurtosis](https://user-images.githubusercontent.com/114852180/227996724-6dc30e33-1b8a-4ff7-92ba-ec48ddf4020e.png)
![df valuecounts](https://user-images.githubusercontent.com/114852180/227996843-6c5d378f-31e2-4089-a641-85c7d6117826.png)

![df2 data](https://user-images.githubusercontent.com/114852180/227997244-0ffb7ed6-97f0-4408-ab77-f93c36472dc0.png)
![df2 datatypes](https://user-images.githubusercontent.com/114852180/227998861-4d9d9793-b18c-42d1-a767-4a638e35b165.png)
![df2 info](https://user-images.githubusercontent.com/114852180/227999402-c2299803-a012-4162-8616-a72e7599c8df.png)
![df2 describe](https://user-images.githubusercontent.com/114852180/227999619-31d2e45e-156b-4a37-9e28-96b697df51cc.png)
![df2 boxplot](https://user-images.githubusercontent.com/114852180/227999856-3c2cab98-c2ff-4466-b76f-f8b687c1b6ba.png)
![df2 countplot](https://user-images.githubusercontent.com/114852180/227999974-4b5ec761-0999-437c-87c4-41021ef5534a.png)
![df2 distplot](https://user-images.githubusercontent.com/114852180/228000169-f0b6d6a7-5fec-4556-b1a6-756571a21472.png)
![df2 value_counts](https://user-images.githubusercontent.com/114852180/228000240-76375bee-1dc1-4fed-ae49-c38ef482781d.png)

# RESULT:
thus the experiment completed sucessfully
