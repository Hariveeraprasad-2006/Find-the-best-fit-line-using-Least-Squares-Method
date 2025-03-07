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
Developed by:Arikatla Hari Veera Prasad
RegisterNumber:212223240014
import matplotlib.pyplot as plt
import numpy as np
x=np.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
numi=0
denom=0
for i in range(len(x)):
    numi=numi+(x[i]-x_mean)*(y[i]-y_mean)
    denom=denom+(x[i]-x_mean)**2
m=numi/denom
c=y_mean-m*x_mean
print("THE SLOPE OF THE LINE IS",m)
print("THE Y INTERCEPT IS ",c)
y_pred=m*x+c
print("THE PREDICTED VALUE IS",y_pred)
plt.scatter(x,y,color="red")
plt.plot(x,y_pred,color="black")
plt.show()
*/
```

## Output:
![image](https://github.com/Hariveeraprasad-2006/Find-the-best-fit-line-using-Least-Squares-Method/assets/145049988/43e714aa-f28b-4b7a-b5ed-1aa419c1a7c3)



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
