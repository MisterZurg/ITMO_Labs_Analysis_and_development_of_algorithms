# Task 3. Algorithms for unconstrained nonlinear optimization. First- and second order methods
## Goal
*The use of first- and second-order methods (Gradient Descent, Non-linear Conjugate Gradient Descent, Newton’s method and Levenberg-Marquardt algorithm) in the tasks of unconstrained nonlinear optimization*

## Problems and methods
*Generate random numbers `α ∈ (0,1)` and `β ∈ (0,1)`. Furthermore, generate the  noisy data `{xk, yk}`, where `k = 0, … , 100`, according to the following rule:*

<center>
    <code>yk = αxk + β + 𝛿k, xk = k / 100</code>
</center>


*To solve the minimization problem, use the methods of Gradient Descent, Conjugate Gradient Descent, Newton’s method and Levenberg-Marquardt algorithm. If necessary, set the initial approximations and other parameters of the methods. Visualize the data and the approximants obtained in a plot separately for each type of **approximant** so that one can compare the results for the numerical methods used. Analyze the results obtained (in terms of number of iterations, precision, number of function evaluations, etc.) and compare them with those from Task 2 for the same dataset*