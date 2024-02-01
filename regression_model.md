# Regression Model

---

First model of this course is called Linear Regression Model. Which means fitting a straight line to your data. Probably the most widely used learning algorithm in the world today.

- Predict the price of the house based on its size.
- Regression model predicts numbers
- Other type is Classification which works with categories (Dog or Cat, Type of disease and whether or not a patient has it)
- Data table is also useful
    - size in feet^2^
    - price in $1000's

Terminology:
- Training Set: Data used to train the model
- Notation:
    - x = "input" variable aka feature
    - y = "output" variable aka "target" variable
    - m = number of training examples 
    - (x, y) = single training example
    - (x^(i)^, y^(i)^) = i^ith^ training example (1^st^, 2^nd^, 3^rd^ ...)
    - in the example x^(1)^ = 2104 y^(1)^ = 400 or (x^(1)^, y^(1)^) = (2104, 400)
    - x^(2)^ != x^2^

Training set:
- input features
- output targets

- feed both to learning algorithm
- the supervised learning algorithm will produce a function f
    - Historically function was called hypothesis
    - Job is to take new input x and output a prediction y-hat
    - function is called the model
    - x is called the input feature
    - the output of the model is the prediction, y-hat
How to represent f?
- f~w,b~(x) = wx + b
- f(x)
- Linear regression with one variable
    - single input variable or feature x
    - Univariate linear regression

# Cost Function Formula 

---

The cost function will tell us how well our model is doing so we can get it to do better.

Training Set
Input features (x)   and    output targets (y)
f~w,b~= wx + b

w,b: parameters

parameters of the model are the variables you can adjust during training in order to improve the model.

w and b are sometimes referred to as coefficients or weights

What do w,b do?

y-hat^i^ = f~w,b~(x^i^)
f~w,b~(x^(i)^) = wx^(i)^ + b

How do you find w,b:
- so that y-hat^(i)^ is close to y^(i)^ for all (x^(i)^, y^(i)^)

**Cost Function**

Squared error cost function = J(w,b) = sum of i=1 to i=m(y_hat^(i)^ - y^(i)^)^2^/2m
m = number of training examples
most commonly used cost function for most regression models

want to find values of w,b that makes the cost function small


simplified
fw(x) = wx (setting parameter b to 0)
parameter = w
cost funtion = J(w) = sum i = 1 ... m (fw(x^(i)^) - y^(i)^)^2^

find value of w that minimizes J(w)

| f~w~(x) | J(w) |
| --- | --- |
| (for fixed w, funtion of x) | (function of w) |