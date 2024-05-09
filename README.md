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
Get the value of X and Y variable

### Step4
Creat the linear regression model and fit

### Step5
predict the CO2 emission where the weight is 2300 kg, and the volume is 1300cm cube

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

![Screenshot 2024-05-09 203908](https://github.com/etjabajasphin/Multivariate-Linear-Regression/assets/152294642/01e8ce51-894c-428e-bf3e-35345b3bf2a0)
![Screenshot 2024-05-09 203937](https://github.com/etjabajasphin/Multivariate-Linear-Regression/assets/152294642/ae5d4df6-d708-47fa-b7fc-7614b1d35c4a)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
