# Train the model with gradient descent

---

Have some function J(w,b) - for linear regression or **any** function
Want min J(w,b)
J(w1,w2,...,wn,b) more parameters 

Outline:
- Start with some w,b
- common choose is (set w=0,b=0)
- keep changing w,b to reduce J(w,b)
- Until we settle at or near a minimum
- may have > 1 minimum
- spin around and find the next baby step to find direction of steepest descent
- until you find yourself at the bottom of the valley
- If you start at a different location you may find a different minimum
- these are called local minima

### Implementing gradient descent

**Gradient descent algorithm**
Repeat until convergence
- when w and b don't change much with each additional step

w = w-a d/dw J(w,b)
b = b - a d/db j(w,b)

- equal sign is assignment operator in this equation (code ==)
- different than truth assertion a = c (value of a is c) a != a + 1
- alpha is aka the **learning rate** small positive number example (0.1) the size of the step down the hill
- Derivative d/dw J(w,b) which direction we want to take our learing step
- simultaneously update w and b

Correct: simultaneous update

tmp_w = w - a d/dw j(w,b)
tmp_b = b - a d/db j(w,b)
w = tmp_w
b = tmp_b

Incorrect
tmp_w = w - a d/dw j(w,b)
w = tmp_w
tmp_b = b - a d/db j(w,b)
b = tmp_b


$\alpha$ is the learning rate
$\frac{ \partial }{ \partial w} J(w,b)$ is the derivative term (partial derivative)

Going through the simpler one parameter version:

$J(w)$
$w = w - \alpha \frac{ \partial }{ \partial w} J(w)$
min = J(w)
This is the parabala 2d example instead of the 3d soup_bowl

The choice of learing rate, $\alpha$ will have a huge impact on the efficiency of your implementation of gradient descent. And if $\alpha$ is chosen poorly gradient descent may not even work at all.


$w = w - \alpha \frac{ \partial }{ \partial w } J(w)$

if $\alpha$ is too small...
- multiply derivative term by a very small baby step
- do decrease the cost J(w) but very slowly
- alot of steps needed to get to the minimum

if $\alpha$ is too large...
- overshoot the minimum
- fali to converge or may even diverge

What if the parameter is already at a local minimum?

Can reach local minimum with fixed learning rate?

- Near a local minumum:
    - Derivative becomes smaller
    - Update steps become smaller
Can reach minimum without decreasing learning rate $\alpha$

### Gradient Descent and Linear Regression

**Linear Regression Model**
$f_{w,b}(x) = wx + b$

**Cost Function**
$J(w,b) = \frac{1}{2m}\sum_{i=1}^m(f_{w,b}(x^{(i)}) - y^{(i)})^{2})$

gradient descent leads to local minimum instead of global minimum

"Batch" gradient descent

Batch: Each step of gradient descent uses all the training examples.

other gradient descent: subsets


