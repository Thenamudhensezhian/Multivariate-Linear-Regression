# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import libraries and load dataset containing multiple input features and one output variable.

### Step2
Separate independent variables and dependent variable:
X = input features
Y = target output

### Step3
Split the dataset into training and testing sets.

### Step4
Train the Linear Regression model using the training data.

### Step5
Predict the output for test data and compare it with the actual output.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))
```
## Output:

<img width="256" height="70" alt="image" src="https://github.com/user-attachments/assets/03b87423-d351-4f8a-b9f8-44e376b6d144" />


<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
