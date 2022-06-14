# DATA-SCIENCE-KDE-PLOT
## AIM:
IMPLEMENT KDE PLOT WITH  OWN DATA SET

## algorithm:

1. read the given data set 
2. import the required packages like  seaborn and label encoder
3. plot the feature bye kde plot


## code:
```
import pandas as pd
import numpy as np
df=pd.read_csv("/content/Placement_Data (1).csv")from sklearn.preprocessing import LabelEncoder
 
# Creating a instance of label Encoder.
le = LabelEncoder()
 
# Using .fit_transform function to fit label
# encoder and return encoded label
label = le.fit_transform(df['status'])

print(label)
#KDE Plot

sns.kdeplot(x="degree_p", data = df,hue='salary')

##  ouput:
![01](https://user-images.githubusercontent.com/94233064/173488244-49684006-2da5-41e0-98ce-17fc1bd90044.png)

### head:
![02](https://user-images.githubusercontent.com/94233064/173488252-18ffa0e5-0e14-44cc-a376-64735453d3fe.png)


## converted numerical value:
![03](https://user-images.githubusercontent.com/94233064/173488267-ddfc27f7-9b8a-41e7-bc3a-18e4ca920f86.png)

## result:
 THUS WE IMPLEMENTED KDE PLOT WITH  OWN DATA SET:
