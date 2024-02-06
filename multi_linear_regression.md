# Multiple Linear Regression

---

| Size in feet$^2$ | # of bedrooms | # of floors | Age of home in years | Price in $1000's |
| --- | --- | --- | --- | --- |
| $x_1$ | $x_2$ | $x_3$ | $x_4$ | |
| 2104 | 5 | 1 | 45 | 460 |
| 1416 | 3 | 2 | 40 | 232 |

 $x_j = j^{th}$ feature

j = 1...4 because we have 4 features
n = number of features
$x^{(i)}$ = features of $i^{th}$ training example

$x^{(2)}$ = [1416 3 2 40] row vector 
$x_j^{(i)}$ = value of feature j in i$^{th}$ training example
$x_3^{(2)}$ = 2

Model:

$f_{w,b}(x) = w_1x_1 + w_2x_2 + w_3x_3 + w_4x_4 + b$

$f_{w,b}(x) = w_1x_1 + w_2x_2 + \cdots + w_nx_n + b$

parameters of the model
$w = [w_1, w_2, w_3, \cdots, w_n]$ called a vector

b is a number

x = [x1  x2 x3 ... xn]

f_w,b (vector x) = vector w * vector x + b

$f_{\overrightarrow{w,b}}(\overrightarrow{x}) = \overrightarrow w \cdot \overrightarrow x + b$

### Vectorization

$f_{\overrightarrow{w,b}}(\overrightarrow{x}) = \overrightarrow w \cdot \overrightarrow x + b$

`f = np.dot(w,x) + b`

- makes code shorter
- runs much faster then without vectorization 
- numpy dot function uses parallel processing

### Gradient Descent for Multiple Linear Regression


##### An alternative to gradient descent

- Normal Eqaution
    - only for linear regression
    - solve for w, b without iterations

- Disadvantages
    - Doesn't generalize to other learning algorithms
    - Slow when number of features is large

- Normal equation method may be used in machine learning libraries that implement linear regression
- gradient descent is the recommended method for finding parameter w,b

