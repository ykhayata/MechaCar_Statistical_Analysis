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

## Summary Stats on Suspension Coils

  For this specific task, we used suspension coils dataset provided. This dataset was made up of 150 different vehicle IDs, 3 different lot numbers, and PSI levels for each vehicle. We then created one summary table to analyze the mean, median, and standard deviation of data. The second table was a table that consisted of the three lots these MechaCars were divided into.
  
<img width="424" alt="totalsum_sus_coils" src="https://user-images.githubusercontent.com/74481469/111112315-2ff40880-851d-11eb-98ef-ed3615337a99.png">

<img width="614" alt="lot_summary_suscoils" src="https://user-images.githubusercontent.com/74481469/111112348-3f735180-851d-11eb-83bc-1e5156fc5274.png">

  When looking at the total summary, we see the current variance is approximately 62.29 PSI which means that it meets the design specification. When looking at the
lots individuals, the first two lots do meet the design specification at a varaince of approximately 0.98 PSI and 7.47 PSI respectfully, though the third lot heavily exceeds the design specification at 170.29 PSI. This tells us the vehicles in lots 1 and 2 should be the main priority for the manufactoring team.

## T-Tests on Suspension Coils 

  In this specific section we want to determine whether or not our manufacturing lots are statistically different than the population mean of 1,500 pounds per square inch. To find the answer, we use R's t.test() function to find four different p-values. We came up with this answer:
  
By using a significance level of 95%, we tested to see if any of the four groups had a statistical difference from the mean of 1,500 PSI. After concluding the tests, we came to the conclusion that all four p-values where significantly greater than .05. This means that we are forced to fail to reject there is a statistical difference between the four groups and the population mean.

Our four tests:

<img width="618" alt="total_pop_test" src="https://user-images.githubusercontent.com/74481469/111113722-6e8ac280-851f-11eb-996a-6bc8c7c18a8e.png">

<img width="550" alt="pop_test1" src="https://user-images.githubusercontent.com/74481469/111113757-79455780-851f-11eb-85eb-f9bf98d65b1c.png">

<img width="521" alt="pop_test2" src="https://user-images.githubusercontent.com/74481469/111113783-83ffec80-851f-11eb-893f-78450e9f5f14.png">

![image](https://user-images.githubusercontent.com/74481469/111113813-8eba8180-851f-11eb-9061-cbf50930caf3.png)











