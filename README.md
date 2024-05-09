# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd

### Step2
Read the csv file

### Step3
Get the value of X and Y varialble

### Step4
create the linaer regression model and fit

### Step5
predict the CO2 emission of car where the weight is 2300kg and the volume is 1300cm cube

## Program:
```
'''
Developed By: G. Pradeep Kumar
Register Number: 212223230150
'''

import pandas as pd
from sklearn import linear_model
data= pd.read_csv("cars.csv")

X = data[['Weight','Volume']]
Y = data['CO2']

regr=linear_model.LinearRegression()
regr.fit(X,Y)

print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)

predictCO2 = regr.predict([[3300,1300]])
print("prediction CO2 for the corresponding Weight and Volume",predictCO2)





```
## Output:

![Screenshot 2024-05-09 203908](https://github.com/pradeep23014186/Multivariate-Linear-Regression/assets/152294642/4db8006b-62dd-451a-acf5-eba027266adb)
![Screenshot 2024-05-09 203937](https://github.com/pradeep23014186/Multivariate-Linear-Regression/assets/152294642/4cb717dc-adea-4b4e-a159-f1709c5c51f2)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
