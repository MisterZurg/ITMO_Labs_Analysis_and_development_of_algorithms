# Task 2. Algorithms for unconstrained nonlinear optimization. Direct methods
## Goal
*The use of direct methods (one-dimensional methods of exhaustive search, 
dichotomy, golden section search; multidimensional methods of exhaustive search, 
Gauss (coordinate descent), Nelder-Mead) in the tasks of unconstrained nonlinear
optimization*
## Problems and methods
***I.** Use the one-dimensional methods of exhaustive search, dichotomy and golden 
section search to find an approximate (with precision `ε = 0.001`) solution 
`x: f(x) → min` for the following functions and domains:*
1. `f(x) = x^3, x ∈ [0, 1]`;
2. `f(x) = |x − 0.2|, x ∈ [0, 1]`;
3. `f(x) = x sin(1/x), x ∈ [0.01, 1]`;

*Calculate the number of `f`-calculations and the number of iterations performed in 
each method and analyze the results. Explain differences (if any) in the results 
obtained.*

***II.** Generate random numbers `α ∈ (0,1)` and `β ∈ (0,1)`. Furthermore, generate the  noisy data `{xk, yk}`, where `k = 0, … , 100`, according to the following rule:*

<center>
    <code>yk = αxk + β + 𝛿k, xk = k / 100</code>
</center>

*where `𝛿k ~ N(0,1)` are values of a random variable with standard normal 
distribution. Approximate the data by the following linear and rational functions:*
1. `F(x, a, b) = ax + b` *(linear approximant)*,
2. `F(x, a, b) = a / (1 + bx)` *(rational approximant)*,

*by means of least squares through the numerical minimization (with precision `ε = 0.001`) of the following function:*

<center>
    <code>D(a, b) = ∑(F(xk, a, b) - yk)^2</code>
</center>

*To solve the minimization problem, use the methods of exhaustive search, Gauss and  Nelder-Mead. If necessary, set the initial approximations and other parameters of the methods. Visualize the data and the approximants obtained in a plot separately for each type of **approximant** so that one can compare the results for the numerical methods used. Analyze the results obtained (in terms of number of iterations, 
precision, number of function evaluations, etc.)*