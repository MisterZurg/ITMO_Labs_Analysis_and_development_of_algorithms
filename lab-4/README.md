# Task 4. Algorithms for unconstrained nonlinear optimization. Stochastic and metaheuristic algorithms
## Goal
*The use of stochastic and metaheuristic algorithms (Simulated Annealing, Differential Evolution, Particle Swarm Optimization) in the tasks of unconstrained nonlinear optimization and the experimental comparison of them with Nelder-Mead and Levenberg-Marquardt algorithms*
## Problems and methods
***I.** Generate the noisy data `(xk, xk)`, where `k = 0, … , 1000`, according to the rule:*
<center>
    <code>
    <table>
        <tr>
            <td></td>
            <td>−100 + 𝛿k</td>
            <td>f(xk) < −100</td>
            <td></td>
        </tr>
        <tr>
            <td>yk = </td>
            <td>f(xk) + 𝛿k</td>
            <td>-100 <= f(xk) <= 100</td>
            <td>xk = 3k / 1000</td>
        </tr>
        <tr>
            <td></td>
            <td>100  + 𝛿k</td>
            <td>f(xk) > 100</td>
            <td></td>
        </tr>
    </table>
    f(x) = 1 / (x^2 - 3x + 2)
    </code>
</center>

*where `𝛿k ~ N(0,1)` are values of a random variable with standard normal distribution. Approximate the data by the rational function*
<center>
    <code>
        D(a, b ,c, d) = ∑(F(xk, a, b, c, d) - yk)^2
    </code>
</center>

*To solve the minimization problem, use Nelder-Mead algorithm, Levenberg Marquardt algorithm and **at least two** of the methods among Simulated Annealing, Differential Evolution and Particle Swarm Optimization. If necessary, set the initial approximations and other parameters of the methods. Use `ε = 0.001` as the precision; at most `1000` iterations are allowed. Visualize the data and the approximants obtained **in a single plot**. Analyze and compare the results obtained (in terms of number of iterations, precision, number of function evaluations, etc.).*

***II.** Choose at least 15 cities in the world having land transport connections between 
them. Calculate the distance matrix for them and then apply the Simulated Annealing
method to solve the corresponding Travelling Salesman Problem. Visualize the
results at the first and the last iteration. If necessary, use the city dataset from*
https://people.sc.fsu.edu/~jburkardt/datasets/cities/cities.htm