# MechaCar Statistical Analysis

## Overview

  The purpose of our analysis is to provide insights on the MechaCar's production in order to assist the manufacturing team. In order to perform this analysis, we  use two datsets that contain information such as miles per gallon and the suspension coils of the MechaCar. We use R and the dplyr library to conduct this analysis. Enjoy!
  
 ## Linear Regression to Predict MPG 
 
  We loaded in the miles per gallon csv dataset and then created a multiple linear regression to determine whether or not we could predict the miles per gallon (mpg) dependent variable by using the vehicle length, vehicle weight, spoiler angle, ground clearance, and all wheel drive independent variables. We came up with this conclusion: 
  
1: The vehicle length and the ground_clearance variables provided a non-random amount of variance, as they both have very small p-values, which translate into a high significance level. But, there are still other factors contributing to variance of the mpg of the MechaCar, as the intercept has a high level of significance.

2: The r-squared value, which is the main indicator of whether the linear model predicts the mpg of the MechaCar is at 0.7149. Because this is out of 100 instances the model would  predict the mpg of the MechaCar correctly approximately 71 times, which is considered effective. 

3: The slope of the linear model is not zero in this case because our linear regression is showing that some independent variables had a significant effect on the dependent variable. Had none of the independent variables had an effect on the dependent variable, then the linear regression would have a near zero slope.

SUMMARY: 

<img width="623" alt="mpglinear_regression" src="https://user-images.githubusercontent.com/74481469/111111829-4baadf00-851c-11eb-9cee-ba2715373c69.png">




