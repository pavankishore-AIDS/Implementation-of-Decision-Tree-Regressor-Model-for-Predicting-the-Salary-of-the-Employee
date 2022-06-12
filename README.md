# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Import pandas modules to start with program.
2.Read csv file and store it in a variable.
3.From sklearn import label encoder to fit attribute.
4.Import train_test_split to get train and test datasets.
5.Using DecisionTreeRegressor predict the value.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: PAVAN KISHORE.M
RegisterNumber:212221230076


import pandas as pd
data=pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["position"])
data.head()
x=data[["position","level"]]
y=data["salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=2))
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)

from sklearn import metrics
mse=metrics.mean_sqaured_error(y_test,y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:
## DATA HEAD AND INFO
![TT1](https://user-images.githubusercontent.com/94154941/173227287-ec2df581-32c4-4584-9a71-a8de23699385.png)
## DATA HEAD
![TT2](https://user-images.githubusercontent.com/94154941/173227302-28f49082-cd5a-40e0-b698-4fe0e444f834.png)
## PREDICTED VALUE
![TT3](https://user-images.githubusercontent.com/94154941/173227314-b2228908-edf3-4256-80b2-59583a360d98.png)



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
