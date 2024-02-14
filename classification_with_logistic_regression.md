# Classification with logistic regression

--- 

Classification

| Question | Answer "y" |
| --- | --- |
| email spam? | no yes |
| is transaction fraud | no yes |
| tumor | malignant benign |

y can only be one of two values
"Binary Classification"

Class Category

fase true
0     1

useful for classification

false/zero = "negative class"
true/one = "positive class"

could try having a threshold for example 0.5

if f_wb(x) < 0.5 -> y_hat = 0
if f_wb(x) >= 0.5 -> y_hat = 1

this won't be accurate becuase of outliers etc.

so linear regression won't work for classification examples

**Logistic Regression**

logistic regression is an s shaped curve

output is always 0 or 1

sigmoid function aka logistic function

horizontal axis takes on both positive and negative values

$g(z) = \frac{1}{1+e^{-z}} 0 < g(z) < 1$

$f_{\overrightarrow{w},b}(\overrightarrow{X})$
$z = \overrightarrow{w} \cdot \overrightarrow{x} + b$

$f_{\overrightarrow{w}, b}(\overrightarrow{X}) = g(\overrightarrow{w} \cdot \overrightarrow{X} + b)$

### Interpretation of logistic regression output

$f_{\overrightarrow{w}, b}(\overrightarrow{X}) = \frac{1}{1 + e^{-(\overrightarrow{w} \cdot \overrightarrow{X} + b)}}$

"probability" that class is 1

Example
x is "tumor size"
y is 0
or 1

f_wb = 0.7
70 percent chance that y is 1

P(y = 0) + P(y = 1) = 1


f_wb(x) = g(w * x + b)

f_wb(x) = g(z) = 1/1+e^(w*x+b)

P(y=1|x:w,b)

0 or 1?

threshold of 0.5

When is f_wb(x) >= 0.5?
When is g(z) >= 0.5
z >= 0
w * x + b >= 0
y_hat = 1

np.dot(x, b) + x < 0
y_hat = 0

**Decision Boundary**

f_wb = g_z = g(w1x1 + w2x2 +b)

z = w * x + b = 0 = Decision Boundary (almost nuetral whether y is 0 or 1)

z = x1 + x2 - 3 = 0
x1 + x2 = 3

Non-linear decision boundaries

