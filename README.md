# MechaCar Statistical Analysis

## Overview

AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. 
AutosRUs’ upper management has called on the data analytics team to review the production data for insights that may help the manufacturing team.
Data Analysis includes the following actions:
- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. 

## Code
MechaCarChallenge.R  [file](MechaCarChallenge.R)

## Linear Regression to Predict MPG

- Vehicle length and ground clearance have p-values of 2.60e-12  and  5.21e-08, respectively , which indicate they are the variables that have the most non-random amount of variance. 
- The slope of the linear model is not zero, as indicated by the overall p-value of 5.35e-11.
- An r-squared value of 0.7149 indicates that the regression model is 71% accurate. This figure would be dependent on the auto manufacturer's threshold for accuracy to be considered good enough.

![MechaCar_mpg_Linear_Regression_statistics](https://user-images.githubusercontent.com/98564776/168491934-646128d3-1635-49c2-bedc-4165b68a8bd7.PNG)


## Summary Statistics on Suspension Coils

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. While the overall variance does meet this criteria  (it is under, at 62.29356 pounds per square inch), the data is skewed by the results from Lot 3, which has a variance of 170.2861224 pounds per square inch, which greatly exceeds the acceptance criteria.

![total_summary](https://user-images.githubusercontent.com/98564776/168491944-42342f5e-0201-4d40-aef8-7f69fec25df7.PNG)

![lot_summary](https://user-images.githubusercontent.com/98564776/168491948-2871d712-de14-4b64-8e45-3a4d7cae125c.PNG)


## T-Tests on Suspension Coils

- Lot 3 is the only lot that shows p-value under .05  which means it is statistically different from the rest.

![One_Sample_T-test](https://user-images.githubusercontent.com/98564776/168491951-9afadd54-f971-40de-92ec-2024d7ae3a50.PNG)


![T-tests_on_each_lot](https://user-images.githubusercontent.com/98564776/168491955-e96a4662-55a4-47ce-ae8d-89327d4f0af6.PNG)

## Study Design: MechaCar vs Competition

- For further study, MechaCar must be measured against the competition. Metrics that would be of interest to a consumer include cost, city or highway fuel efficiency, horse power, maintenance cost, safety rating, rear leg room, comfort, cargo space, and interior add-ons.  
- City or highway fuel efficiency, cost, cargo space and safety ratings would be interesting metrics to test against competing models. 
- T-tests would be the best statictical tests to run. 

### Resources

- MechaCar_mpg.csv   [file](MechaCar_mpg.csv)
- Suspension_Coil.csv  [file](Suspension_Coil.csv)
- RStudio
