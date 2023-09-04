# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: A.J.PRANAV
RegisterNumber: 212222230107
*/
import matplotlib.pyplot as plt
import numpy as np
X=np.array([0,1,2,3,4,5,6,7,8,9])
Y=np.array([1,3,2,5,7,8,8,9,10,12])
Xbar=sum(X)/len(X)
Ybar=sum(Y)/len(Y)
m=n=d=0
for i in range(len(X)):
  n+=(X[i]-Xbar)*(Y[i]-Ybar)
  d+=(X[i]-Xbar)**2
m=n/d
c=Ybar-m*Xbar
print(m,c)
plt.scatter(X,Y,color='red')
Y_pred=m*X+c
print(Y_pred)
plt.plot(X,Y_pred)
plt.show()
```

## Output:
![image](https://github.com/Pranav-AJ/Find-the-best-fit-line-using-Least-Squares-Method/assets/118904526/18e49e06-c098-4a53-ba5a-e622cb526300)


## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
