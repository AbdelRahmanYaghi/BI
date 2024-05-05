# Decision Analysis (Without Proba)
## Example: Pittsburhg development 
* Plan to build one of these three projects:
    * One project with 30 condos
    * One project with 60 condos
    * One project with 90 condos
* Future event is the chance event concerning the demand for the condos.
* The financial success depends on the condos size   
* To solve this, one should do one of the following methods:
### Payoff Tables
1) Decision alternatives (How many condos?) 
2) Chance event (States of nature, i.e. Weak demand, or Strong Demand)
3) You then create a table with the columns being States of nature, and the rows being the decision alternatives. Like the table below.
4) Then based on the tables, you can apply 3 different options.
    * Minimax Regret ; Regret = (a_max - a_i). <br>
     For example, <br> Strong Demand, and Small Condo, will have a regret of 20 - 8 = 12. <br> Weak Demand, and Medium Condo, 7 - 5 = 2
    * Optimistic:  Takes the highest one from the Strong demand. 
    * Conservative: Takes the highest one from the Weak demand.

<table>
  <thead>
    <tr>
      <th>Decision Alternatievs</th>
      <th>Strong Demand</th>
      <th>Weak Demand</th>
    </tr>
  </thead>
  <tbody>
    <tr>
    <td>Small Condos $d_1$</td>
    <td>8</td>
    <td>7</td>
    </tr>
    <tr>
      <td>Medium Condos d2</td>
      <td>14</td>
      <td>5</td>
    </tr>
    <tr>
      <td>Large Condos d3</td>
      <td>20</td>
      <td>-9</td>
    </tr>
  </tbody>
</table>


### Decision Tree
1) Decision alternatives (How many condos?) 
2) Chance event (States of nature, i.e. Weak demand, or Strong Demand)
3) Create a tree, where (Check slides lol, I will not be bothered to write the tree here.)

# Decision Analysis with Probs:
  * Expected value: If you had the probabilities for each event to occur, then you mutliple the chance of X occuring by the "profit" if X occured. 
  * Risk: Probability mass function, for example:
    * 8 mil, if Event 1 occured
    * 2 mil, if Event 2 occured
    * -4 mil, if Event 3 occured

  * Sensitivity Analysis: How much change is required for the optimal solution to stay optimal. 


# Decision Analysis with Sample Information:
## Example: PDC Management
* Decision Strategy - Metric 1: EVSI -> Expected Value of Sample Information
  * Done by reducing the branches over and over \sum(prob * value).
  * ***In this example, we took the maxes.
* Decision Strategy - Metric 21: EVPI -> Expected Value of Perfect Information
  * If you will what probability will hit.  
  * Done by 0.8 * 20 + 0.2 * 7. We got this by knowing that if High demand occurs (80%) we will get large complex (20 mil), and if Low demand occurs (20%) we will get the small complex (7 mil), 

# Computing Brach Probability with Bayes' Theorom
* Join prob: prob that A & B happens at the same time (AND): $P(A \cap B)$ This equals $P(B) P(A|B) = P(A) P(B|A)$
  * If A and B are independant, then $P(A \cap B) = P(A) P(B)$ 
* Join prob: prob that A or B happens at the same time (OR): $P(A \cup B)$. This equals $P(A) + P(B) - P(A \cap B)$
* Conditional Probability: Prob of A given B. $P(A | B)$. This equals $\frac{P(A \cap B)}{P(B)} $
  * If A and B are independant, then $P(A | B) = P(A)$
<!-- * If A and B are mutually exclusice  -->
* Bayes Theorem: $P(A|B) = \frac{P(B|A) P(A)}{P(B)}$
* Bayes Theorem Final Form: $P(B_i|A) = \frac{P(A|B_i) P(B_i)}{\sum_{i=1}P(A|B_i) P(B_i)}$
  * *Assuming the all i in A are independent.

