Standard Form main features:
* Always Mamimize
* Non-Negative Decision Variables
* Non-Negative Right Hand Side of Constraints
* All constraints should be equality

How to deal with:
<h4>Minimize</h4>
<p>Multiply objective function with (-1)</p>

____

<h4>Non Negative RHS in Constraint</h4>
<p>Multiply both sides with (-1) and flip the < to >, and vice versa.
For Example:

$Ax \geq -b$

Becomes

$-Ax \leq b$
<p>

____

<h4>Greater than or equal in Constraint (Slack Variable)</h4>
Change constraint from

$Ax \geq b$

Becomes 

$Ax - e = b$

Subject to

$e \geq 0$

____
<h4>Less than or equal in Constraint (Excess Variable)</h4>
Change constraint from

$Ax \leq b$

Becomes 

$Ax + e = b$

Subject to

$e \geq 0$

____

<h4>Non Postive Decision Variable</h4>
**CHECK THIS AGAIN**

This:

$xA = b$

$x \leq 0$


Becomes:

$-x^\prime A = b$

$x^\prime \geq 0$


____

<h4>Unrestricted Decision Variable</h4>
This:

$Ax = b$

$x\;urs$ (Means Unsrestricred)

Becomes:

$x = x^\prime - x^{\prime}{^\prime}$ 

where

$x^\prime, x^{\prime}{^\prime} \geq 0$

So

$A(x^\prime - x^{\prime}{^\prime}) = b$

___

Example 1:

$\mathrm{minimize} -4x_1 + x_2 + x_3$<br>
Subject To <br>
$3x_1 + x_2 + x_3 \leq 6$<br>
$-2x_1 - x_2 + x_3 \leq -3$<br>
$x_1 + x_2 - x_3 \geq 6$<br>

$x_1 \geq 0, \; x_2 \leq 0, \; x_3 \;urs$<br>

Becomes:

$\mathrm{maximize} \; 4x_1 - x_2 - x_3$<br>
Subject To <br>
$3x_1 - x_2^\prime + (x_3^{\prime} - x_3^{\prime}{^\prime})  + e_1 = 6$<br>
$2x_1 - x_2^\prime - (x_3^{\prime} + x_3^{\prime}{^\prime}) - e_2 = 3$<br>
$x_1 - x_2^\prime - (x_3^{\prime} + x_3^{\prime}{^\prime}) - e_3 = 6$<br>
$e_1, e_2, e_3 \geq 0$<br>
$x_2^\prime, x_3^{\prime}, x_3^{\prime}{^\prime} \geq 0$<br>
$x_1 \geq 0$


___

Example 2 (ORIGINAL - ALREADY STANDARIZED - Primal Dakota Problem):

$\mathrm{maximize} \; 60x_1 + 30x_2 + 20x_3$<br>
Subject To <br>
$8x_1 + 6x_2 + x_3 \leq 48$<br>
$4x_1 + 2x_2 + 1.5x_3 \leq 20$<br>
$2x_1 + 1.5x_2 + 0.5x_3 \leq 8$<br>

$x_1, x_2, x_3 \geq 0$<br>

Becomes:

$\mathrm{maximize} \; 4x_1 - x_2 - x_3$<br>
Subject To <br>
$3x_1 - x_2^\prime + (x_3^{\prime} - x_3^{\prime}{^\prime})  + e_1 = 6$<br>
$2x_1 - x_2^\prime - (x_3^{\prime} + x_3^{\prime}{^\prime}) - e_2 = 3$<br>
$x_1 - x_2^\prime - (x_3^{\prime} + x_3^{\prime}{^\prime}) - e_3 = 6$<br>
$e_1, e_2, e_3 \geq 0$<br>
$x_2^\prime, x_3^{\prime}, x_3^{\prime}{^\prime} \geq 0$<br>
$x_1 \geq 0$


