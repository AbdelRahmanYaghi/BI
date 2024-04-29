Time series patterns:
1. Horizontal Pattern: The mean is equal over any time period
2. Trend: "Continuous?" Long Term Overall change, whether increasing or decreasing.
3. Seasonal Pattern: The Non-Random behaviour and pattern across a period of time.
4. Trend and Seasonal Pattern: 2+3
5. ...

A. Horizontal Pattern:
    - Stationary: Statistics are independent from the time variable.
      * Plotting a Stationary will always result in a Horizontal with minor changes.
      * E.g. Gasoline Problem

B. Trend Pattern:
    * E.g. Bicycle Sales
    * E.g. Cholesterol Drug Revenue

C. Seasonal Pattern:
    * E.g. Umbrella Sales

D. Trend and Seasonal Pattern:
    * E.g. Smartphone Sales

Exponential Smoothing closed form: $\hat{y}_{t+1} = \alpha \sum_{i=0}^{t-2}((1−\alpha)^{i}y_{t-i}) + (1-\alpha)^{t-1}y_1$

*** Check Gallery for changing a seasonality to a multivariate problem. Also, in slide 10/19 of chpt 8
*** CHECK SHADOW PRICES. THEIR FUNCTIONS IN DOCPLEX
*** FORMULATION ==> CHECK HOW TO FORMULATE IN VERSION 0. & HOW TO GENERALIZE BASIC PROBLEMS.
*** WHAT IS CLOSED FORM? OR ITERATIVELY? EXPONENTIAL SMOOTHING EQUATION.