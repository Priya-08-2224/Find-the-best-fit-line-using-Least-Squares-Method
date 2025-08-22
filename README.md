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
Developed by: Priyadharshini J
RegisterNumber:  212224230210

import numpy as np
import matplotlib.pyplot as plt

# Very simple implementation
def simple_linear_regression():
    # Hardcoded sample data
    X = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
    y = np.array([2, 4, 5, 4, 6, 7, 8, 9, 10, 12])
    
    # Calculate means
    mean_X = np.mean(X)
    mean_y = np.mean(y)
    
    # Calculate slope and intercept
    numerator = sum((X - mean_X) * (y - mean_y))
    denominator = sum((X - mean_X) ** 2)
    slope = numerator / denominator
    intercept = mean_y - slope * mean_X
    
    print(f"Slope: {slope}")
    print(f"Intercept: {intercept}")
    print(f"Equation: y = {slope:.2f}x + {intercept:.2f}")
    
    # Plot
    plt.scatter(X, y)
    plt.plot(X, slope * X + intercept, color='black')
    plt.show()

# Run the simple version
simple_linear_regression()
*/
```

## Output:
<img width="1036" height="660" alt="Screenshot 2025-08-22 214457" src="https://github.com/user-attachments/assets/167cfc23-5a33-4590-beb9-46cb5f78db77" />



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
