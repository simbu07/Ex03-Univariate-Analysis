# Ex03-Univariate-Analysis
## Aim:

 To read the given data and perform the univariate analysis with different types of plots.
## Theory:

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
## Algorithm:

### Step 1:

Read the given data.
### Step 2:

Get the information about the data.
### Step 3:

Remove the null values from the data.
### Step 4:

Mention the datatypes from the data.
### Step 5:

Count the values from the data.
### Step 6:

Do plots like boxplots,countplot,distribution plot,histogram plot.
Program:
```
Developed By : Silambarasan K
Reg No: 212221230101
```
```python

import pandas as pd
import numpy as np
import seaborn as sns

data=pd.read_csv('SuperStore.csv')
data

data.head()

data.info()

data.describe()

data.isnull().sum()

data.dtypes

data['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=data)

sns.countplot(x='Postal Code',data=data)

sns.distplot(data["Postal Code"])

sns.histplot(x='Postal Code',data=data)


```
## Output:
### Dataset:
![dataset](https://user-images.githubusercontent.com/94525786/229038797-4b3c7c79-1a7a-4665-98b9-a1c55af0d1db.png)

### Head data:
![head](https://user-images.githubusercontent.com/94525786/229038310-5c65a9cf-1be8-47e8-8a6b-510e54508739.png)

### Dataset Information:
![info](https://user-images.githubusercontent.com/94525786/229038295-c3bc7589-f727-47db-8b15-c19d74c985c5.png)

### Data Description:
![describe](https://user-images.githubusercontent.com/94525786/229038331-94d0d748-4981-4ad9-a19a-07905810fef6.png)

### Null data:
![null](https://user-images.githubusercontent.com/94525786/229039704-dc256651-d147-40ae-8b34-78aab416f466.png)


### Datatype & Value counts:
![dtype](https://user-images.githubusercontent.com/94525786/229038317-32dd15ed-44b3-4877-a245-7eed39630e89.png)

### Box plot:
![boxplot](https://user-images.githubusercontent.com/94525786/229038387-5041f352-65d6-4e0f-a24c-1dbbdbdd10d4.png)

### Count plot:
![countplot1](https://user-images.githubusercontent.com/94525786/229038381-19a26daa-65bc-4bae-8463-23f6c1ba3129.png)

### Distribution plot:
![displot](https://user-images.githubusercontent.com/94525786/229038320-36dc7999-5752-4db7-a255-a2742bcddcd6.png)

### Histogram plot:
![histoplot](https://user-images.githubusercontent.com/94525786/229038307-a1aa6984-4b68-4bba-8171-9d6828c2160d.png)


## Result:

Thus, we have read the given data and performed the univariate analysis with different types of plots.




