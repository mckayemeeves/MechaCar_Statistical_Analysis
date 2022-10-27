# MechaCar_Statistical_Analysis
## Purpose of Analysis
- AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.
## Overview
- In this analysis I will perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers.

## Linear Regression to Predict MPG
* Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
  - Vehicle length and vehicle ground clearance have impact on the cars MPG when looking at the mechacar prototype. On the other hand, the car weight, AWD, and spoiler angle show that their p-values have a random amount of variance with the dataset.
* Is the slope of the linear model considered to be zero? Why or why not?
  - The P-value for this analysis is 5.35e-11, which is really small compared to .05% (the significance level). Therefore we should reject our null hypothesis because the slope of the linear model is not zero
* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
 - The r-squared value is .7149. This tells us that the majority of the MPG predictions (71%) will be based on this model. But this shows that it is not an effective way to predict the MPG.
![Screen Shot 2022-10-26 at 8 00 46 PM](https://user-images.githubusercontent.com/106174279/198176339-5378c565-8e84-47fb-89ef-b93d3f042757.png)
![Screen Shot 2022-10-26 at 8 08 02 PM](https://user-images.githubusercontent.com/106174279/198176363-c4198de5-eaef-47fb-90cb-9ce99aaf56a2.png)

## Summary Statistics on Suspension Coils
* The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.

- Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
  - The variance of the coils is 62.29 PSI, which is within the 1000 PSI variance requirement. The table below shows the difference between the three lots. 
![Screen Shot 2022-10-26 at 8 09 55 PM](https://user-images.githubusercontent.com/106174279/198176279-83da83c2-23fa-4407-b062-c1d398744a77.png)

## T-Tests on Suspension Coils 
Summary of t-test results across all manufacturing lots and for each lot
- The true mean of the sample is 1498.78
- The p-value is .06 (higher than common significance level of .05)
Therefore there is not enough evidence to compel me to reject the null hypothesis because all three of the manufacturing lots are statistically similar to the population mean of 1500
![Screen Shot 2022-10-26 at 8 10 36 PM](https://user-images.githubusercontent.com/106174279/198176306-0c349df9-cf7d-4021-89b7-c15fff95dfc1.png)

## Study Design: MechaCar vs Competition
### Summary of test hypothesis
What metric or metrics are you going to test?
- MPG
- Drive Package
- Current price
- Resale Value
- Engine Type
- Maintenance cost
- Safety Feature Rating
What is the null hypothesis or alternative hypothesis?
- Null Hypothesis: MechaCar is priced correctly based on its performance of key factors for its genre.
- Alternative Hypothesis: MechaCar is NOT priced correctly based on performance of key factors for its genre.
What statistical test would you use to test the hypothesis? And why?
- A multiple linear regression would be used to determine the factors that have the highest correlation/predictability with the list selling price (dependent variable); which combination has the greatest impact on price (it may be all of them!)
What data is needed to run the statistical test?
- This study would involve collecting data on MechaCar and its comparable models across several different manufacturers over the last 3 years. In order to run this, I would need the following data- competitions' comparable models,
The competing MechaCars, and the factors to look at in order to find out a good price to sell the cars.
