# Decision Analysis
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
