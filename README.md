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
Get the value of X and y variables

### Step4
Create the linear regression model and fit.

### Step5
redict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube

## Program:
```
Developed by: MUKESH D
Register number: 212224040204

import pandas as pd 
from sklearn import linear_model 
df=pd.read_csv("car (1).csv") 
x=df[['Weight', 'Volume']] 
y=df['CO2'] 
regr=linear_model.LinearRegression() 
regr.fit(x,y)  
print('Coefficients:',regr.coef_) 
print ('Intercept:', regr.intercept_) 
predictedCO2=regr.predict([[3300,1300]]) 
print("predicted co2 for the correspin weight and vol, ",predictedCO2)








```
## Output:

<img width="1410" height="494" alt="image" src="https://github.com/user-attachments/assets/92e0a125-2cb5-4a07-a86b-53fa09417f4a" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
