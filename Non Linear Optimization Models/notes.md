What does this mean >> "Convex region: For any 2 points in the region, any convex combination should be between them"???

* Convex combination= l*x_1 + (1-l)* x_2 where l is lambda.
* "Reduces cost" in Non linear is called "Reduced Gradiant".


Local and Global Optimality:
* We used to have one name for optimal solution. Just the optimal solution for all the problems
* You can face problems where the optimal solution for the problem in Non Linear is infeasable (Global Optimality is infeasable).
* Hence, we try to look for Local Optimality, meaning the optimal solution whithin the neighborhood for the answer.

Local Optima:
* A feasible solution when there are no other feasible points with a better objective function value in the neighborhood region.

Shapes (u (cup), n (cap), __ (line)):
u is convex
n is concave
u, n, and __ all together are convex and concave.

DOCPLex can't do some of these probelms, hence, you have to derivate based on X = 0 and Y = 0.  

* Forcasting adoption of a new product:
    * Inputs:
        * M = the number of people estimated to eventually adopt the new product
        * q = the coef of imitation
        * p = the coef of innovation
    * Function:
        * F_t = (p + q[C_{t-1}/m])(m-C_{t-1})
