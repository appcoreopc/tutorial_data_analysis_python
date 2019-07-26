# tutorial_data_analysis_python

Import libraries 

~~~ python 

import seaborn as sb
import pandas as pd
import matplotlib.pyplot as plt

~~~~

Getting your data source sample 

~~~python 

 df = sb.load_dataset('tips')

~~~

try typing "df" and see what it looks like 

~~~python
df
~~~~

### Working with data

Now that you have seen, basic layout of dataframe and what it looks like 


#### Cross tab - provides tabular and categorical information of specific column  

pd.crosstab(df.sex, df.smoker)
       
sex     |     smoker|  Yes  No|
--- | ---|---
Male     |     60     |  97|
Female   |     33   |    54|





### Plotting of charts 

seaborn.barplot(x="day", y="size", data=df)
plot.show()
