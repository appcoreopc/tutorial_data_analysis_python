# tutorial_data_analysis_python

Import libraries 

~~~ python 


~~~~

Getting your data source sample
import seaborn as sb
import pandas as pd
import matplotlib.pyplot as plt 

~~~python 

 df = sb.load_dataset('tips')

~~~

try typing "df" and see what it looks like 

~~~python
df
~~~~

### Working with data

Fiddling with your data 


df.columns -> you get a list of all your columns 

To see specific colums 

> df.tip

To list first five columns 


> df.head()


To take the top n rols 

> df.head(20)



To get data types of columsn 

> df.datatypes


To view a specific recrord by index

> df.iloc[1]

where 1 is the reord number 


''Select row by column condition''

>df.loc[df['size']==10]


## Other operation 

Get all value in a dataframe as a numpy array

> df.values 





Group by 

When you issue this command, pandas automatically sum ups all the numerical values group by sex. 

> df.groupby(['sex']).sum()


Merge is a cool feature. 

It merges data from 2 data frame and does record matching automatically.


Create new column 

To create a new column, assign a new name for it, as show in code below and it will take value "value_to_take".

> df["newcolumn_name"] = value_to_take


Create new row 

Update a row 

Update column value 

Update column value based on criteria


Now that you have seen, basic layout of dataframe and what it looks like 


#### Cross tab - provides tabular and categorical information of specific column  

pd.crosstab(df.sex, df.smoker)
       
sex/smoker    |  Yes | No|
--- | ---|---
Male     |     60     |  97|
Female   |     33   |    54|





### Plotting of charts 

seaborn.barplot(x="day", y="size", data=df)
plot.show()



### Scatter plot 


Here, we trying to see how data distribution looks like :- 

plt.scatter(df.tip. df.sex)
plt.show()


### Confuson martix


### Importance of feature 








