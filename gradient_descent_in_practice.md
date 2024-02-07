# Gradient Descent In Practice 

---

- Feature and parameter values
    - price - w1x1 + w2x2 + b
    - x1: size (feet$^2$) range: 300 - 2000  
        - large range of values
    - x2: # bedrooms range: 0-5   
        - small range of values
    - House: x1 = 2000, x2=5, price 500000

    Size of parameters w1, w2?

    w1 = 50 w2 = 0.1 b = 50

    price = 50 * 2000 + 0.1 * 5 + 50
    price = 100,050,500

    w1 = 0.1 w2 = 50 b = 50

    price = 0.1 * 2000 + 50 * 5 + 50
    price = 500,000

    if possible values of feature are large then values of parameter will be reletively small

    would be helpful to scale the features
    0 to 1 range for both
    contour plot will look more like a circle than a tall and skinny oval

    $300 \leq x_1 \leq 2000$

    $x_{1,scaled} = \frac{x_1}{2000}$

    $0.15 \leq x_{1,scaled} \leq 1$

    $0 \leq x_1 \leq 5$

    $x_{1,scaled} = \frac{x_1}{5}$

    $0 \leq x_{1,scaled} \leq 1$

    Mean Normalization

    find average of $x_1$
    $\mu_1$
    $x_1 = \frac{x_1-\mu_1}{2000 - 300}$

    $-0.18 \leq x_{1} \leq 0.82$

    do the same with $\mu_2$

    $-0.46 \leq x_{1} \leq 0.54$

    Z-score normalization

    standard deviation $\sigma$

    $x_1 = \frac{x_1-\mu_1}{\sigma_1}$

     $-0.67 \leq x_{1} \leq 3.1$

     $x_2 = \frac{x_2-\mu_2}{\sigma_2}$

    $-1.6 \leq x_{1} \leq 1.9$

    Feature Scaling

    - aim for about $-1 \leq x_{j} \leq 1$ for each feature $x_j$

    Checking gradient descent for convergence
    - J(w,b) over # iterations graph
    - Automatic Convergence test
        - Let $\epsilon$ "epsilon" be $10^{-3}$
        - If J(w,b) decreases by $\leq \epsilon$ in one iteration declare convergence
        - (found parameters w,b to get close to global min)

    
Choosing the learning rate


