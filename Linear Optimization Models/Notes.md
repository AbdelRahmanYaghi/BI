# LINEAR PROGRAMMING (Polynomial Time)
- Decision Variables --> Continuous
- Constraints --> Linear
- Objective Function --> Linear

IF Decision VARIABLES ARE INTEGER, 
THEN IT IS INTEGER LINEAR PROGRAMMING (Exponential Time) 

## BI problems:
- A- Stochastic
- B- Determenistic
    - a- Linear
        1- Linear Programming
        2- Integer Linear Programming
    - b- NonLinear
        1- Non Linear Programming
            1- Convex (Solvable)
            2- Non-Convex (Not Solvable)
        2- Integer Non Linear Programming
            x- B INLP

## Special Cases of solutions:
- A- Alternative Optimal Solution
- B- Infeasibility
- C- Unbounded 

## Convex (Linear) Combination:
Any point between 2 points given by:
Y = Lx1 + (1-L)x2,
where L is lambda, any number between 0-1

## Lets say:

Maximize cx
s.t. Ax <= b

## Change in A:
??? What happens

## Change in b:
Each constraint has a shadow price:
- Which is the rate/ or amount of change on the objective value
for each [1] unit increase in the right hand side of a constraint.

Binding constraint:
When the values of the optimal decision variable values in a constraint
it will exactly be on the limit of that constraint. e.g.
    DV:  a = 2, b = 4.
    Constraint: 2a + 1b <= 8 ---> Binding Constraint

- Non Binding Constraint will always have a shadow price of 0.
- Shadow prices of constraints where e.g. S>=0 or S<=20 is called "Reduced Cost of S".

## Change in c:
Allowable Increase and Allowable Decrease:
Indicates the change in objective function coef for which the current solution
- will remain optimal.

HMW: Apply Allowable Increase and Decrease + Check built-in commands for the ShadowPrice.

- Variance of return is the risk
- The more you increase the projected return, the more risk you get.
- In portfolio selection:
    - increase return without risk increasing above a certain threshold.
E.g:
    - Minimize the risk expected
    S.T. 
    Return >= A
or
    - Maximize the return expected
    S.T. 
    Risk <= A

## There is a difference between optimal solution and optimal decision variable values.
Optimal objective function value is the evaluation for the optimal decision variables.
Solution refers to the optimal Decision variables values.

## Generating An alternative optimal solution:
Doable by changing the Linear program such that it aims to maximize or minimize
other decision variables. While adding a constraint dictating that the solution
should be equal to the optimal solution.
