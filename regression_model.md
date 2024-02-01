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


