# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Gather your data points. You need two sets of values: one for the input (independent variable, X) and other for the output (dependent variable, Y).
2.Set initial values for the parameters of the model, such as the slope 𝑚 intercept b of the regression line. You can start by initializing these to zero or small random value
3.For any input x, the model predicts and output y_pred
4.For each data point, calculate the error between the actual output y and the predicted output y_pred
5Adjust the values of m and b to minimize the error
6.Iterate over the dataset multiple times repead=ting steps 3-5 until the parameters stabilize and error become sufficiently small
7.Once the model has been trained use the final values of m and b to predict the output for new input 

## Program:
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: swetha R
RegisterNumber: 212223040221

import numpy as np
import matplotlib.pyplot as plt
X=np.array(eval(input("Enter X value:")))
Y=np.array(eval(input("Enter Y value:")))
X_mean=np.mean(X)
Y_mean=np.mean(Y)
num=0
denom=0
for i in range(len(X)):
    num+=(X[i]-X_mean)*(Y[i]-Y_mean)
    denom+=(X[i]-X_mean)**2
m=num/denom
b=Y_mean-m*X_mean
print("The m value is: ",m)
print("The b value is: ",b)
y_predicted=m*X+b
print("The Y_Predicted value is: ",y_predicted)

print("Slope: ",m)
print("y-intercept: ",b)
plt.scatter(X,Y)
plt.plot(X,y_predicted,color='pink')

plt.xlabel("Hours")
plt.ylabel("Score")
plt.title("Hours VS Scores")
plt.show()


## Output:
![expt 1](https://github.com/user-attachments/assets/3ebca8e6-eed9-426e-8509-9b8f8323cf56)

![exp1](https://github.com/user-attachments/assets/59d31b61-9918-4ac3-8392-85cdeba0c32d)




## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
