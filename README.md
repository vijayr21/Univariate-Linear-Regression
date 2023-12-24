# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.

4.	Compute the y -intercept of the line by using the formula:

5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
#Program to implement univariate Linear Regression to fit a straight line using least squares.
#Developed by: VIJAY R
#register number: 23013759

import numpy as np 
import matplotlib.pyplot as plt
x = np.array([0,1,2,3,4,5,6,7,8,9])
y = np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
xmean = np.mean(x)
ymean = np.mean(y)
num=0
den=0
for i in range(len(x)):
    num+=(x[i]-xmean)*(y[i]-ymean)
    den+=(x[i]-xmean)**2
m = num/den
b = ymean - m*xmean
print(m,b)
ypred = m*x+b
print(ypred)


plt.scatter(x,y,color='Red')
plt.plot(x,ypred,color='Blue')
plt.show()


```
## Output
![Screenshot 2023-12-24 214220](https://github.com/vijayr21/Univariate-Linear-Regression/assets/149347607/ae464f7e-9f7f-48bf-a19a-a25866a9fa9f)

![Screenshot 2023-12-24 214240](https://github.com/vijayr21/Univariate-Linear-Regression/assets/149347607/9a7c983d-2985-4992-a8ce-7580809e9f92)
![Screenshot 2023-12-24 214250](https://github.com/vijayr21/Univariate-Linear-Regression/assets/149347607/158cd1cd-18de-4244-ada4-ff9479ca78bb)



## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
