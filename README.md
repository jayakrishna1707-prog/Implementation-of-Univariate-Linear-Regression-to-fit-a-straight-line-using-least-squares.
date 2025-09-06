# Implementation of Univariate Linear Regression to fit a straight line using least squares.
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.
# Equipments Required:
1.hardware - PCs
2.Anaconda – Python 3.7 Installation / Jupyter notebook
# algorithm
1.Get the independent variable X and dependent variable Y.
2.Calculate the mean of the X -values and the mean of the Y -values.
3.Find the slope m of the line of best fit using the formula.

<img width="309" height="137" alt="image" src="https://github.com/user-attachments/assets/4102a1b0-18cb-4d8c-b8c1-ab25ab57cbf9" />

4.Compute the y -intercept of the line by using the formula:

<img width="196" height="53" alt="image" src="https://github.com/user-attachments/assets/85555b14-ec50-4c84-8a79-ab33ef6a764e" />

5. Use the slope m and the y -intercept to form the equation of the line. 6. Obtain the straight line equation Y=mX+b and plot the scatterplot.
# Program:
```
import numpy as np 
import matplotlib.pyplot as plt 

x = np.array(eval(input()))
y = np.array(eval(input()))
```

 <img width="264" height="40" alt="image" src="https://github.com/user-attachments/assets/092966db-b2a4-4b62-bc1f-ff68d94577ad" />

```
x_mean = np.mean(x)
y_mean = np.mean(y)
num = 0
denom = 0 
for i in range(len(x)):
    num+= (x[i] - x_mean) * (y[i] - y_mean)
    denom += (x[i] - x_mean)**2
m = num/denom
b = y_mean - m * x_mean
print(m,b)
```

<img width="350" height="23" alt="image" src="https://github.com/user-attachments/assets/317ac668-73d4-4d99-9100-c3c7060399b5" />
```


y_predicted = m* x + b 
print(y_predicted)
```


<img width="651" height="47" alt="image" src="https://github.com/user-attachments/assets/a44b346d-e879-4ccd-99e2-eddf2eb69dfc" />
```
plt.scatter(x,y)
plt.plot(x,y_predicted,color='red')
plt.show()
```
# output


<img width="698" height="518" alt="image" src="https://github.com/user-attachments/assets/a129a58a-0b70-419e-b0b2-fcc9465e9db1" />

# Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.











