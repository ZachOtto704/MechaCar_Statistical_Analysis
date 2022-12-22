# MechaCar Statistical Analysis


## Linear Regression to Predict MPG

![image](https://user-images.githubusercontent.com/112716673/209240642-5310ebd2-9093-4409-bf8a-db269eef77b4.png)

When looking at the data output above, it is important to note that the "Pr(>/t/)" column represents the probability that the car attribute will create an amount of variance. The two smallest vallues are ground clearance and vehicle length, so these must me the attributes that are creating the variance.

![image](https://user-images.githubusercontent.com/112716673/209241211-ca0df780-254f-4214-94e4-e47869820511.png)

The slope of the linear model, will not be zero. In looking at the data output above, we can see that there are variables with non-zero coefficient values, (ground clearance and vehicle length) so the linear model will not have a slope of zero.

This data has been proven to be relatively effective in predicting mpg. It can be seen that there are strong coefficients with vehicle length and ground clearance. Also, the multiple R-squared value is .7149. Meaning that there is a 71% chance that the combination of the factors we looked at will affect mpg.

## Summary Statistics on Suspension Coils

The total_summary variable (reflecting data across all 3 lots) has a variance of 62, which is acceptable by falling within the 100 pound variance amount. When looking at specific lots, we see that lot 1 and lot 2 have variance of 1, and 7.5 respectively. Both of which are acceptable by falling within the 100 pound variance limit. Lot 3, however, has a variance of 170. This is unacceptable as it lie0 pound variance limit. 

## T-Tests on Suspension Coils

Below are the T Tests I ran to compare the means of our suspension coil samples vs. the expected mean of 1500 PSI.

![image](https://user-images.githubusercontent.com/112716673/209235743-db20bbfe-746b-41f1-a7eb-c7f4364f28e4.png)

This was the sample for all 3 lots. We can see that the p value is .095, which is greater than our significance value of .05

![image](https://user-images.githubusercontent.com/112716673/209235811-9ec3cc0c-9b70-4249-8e29-89290bb04e84.png)

This was the sample for lot 1. We can see the p value here is .48, which is greater than our significance level of .05

![image](https://user-images.githubusercontent.com/112716673/209235858-ebc2c029-6ef3-4e27-94a8-4c865e4c9a60.png)

This was the sample for lot 2. We can see the p value here is .34, which is greater than our significance level of .05

![image](https://user-images.githubusercontent.com/112716673/209235901-350c00e1-ded0-432d-ae49-1a02ff79f664.png)

This was the sample for lot 3. We can see that the p value is .14, which is greater than our significance level of .05


## Study Design: MechaCar vs Competition

To compare the MechaCar to its competition, we will look at the follwing metrics:

-Price
-Combined MPG
-Horsepower

Our null hypothesis is that the MechaCar is not competitively priced compared to its competition based on MPG, and horsepower. 
Our alternate hypothesis is that the MechaCar is competitively priced compared to its competition based on MPG, and horsepower.

A good test to run in this case would be to comnmpare how the Mechacar compares on price with an equation in the test like ((mpg/price)+(hp/price)). Finding the variance in the value from the equation between the Mechacar and its competition can be found with a t test. This would be a good test to run to see if the Mechacar is overpriced, underpriced, or just right. 

The data for this test would be found from Mechacar's database, and would be compared against a database of other vehicles price, mpg, and hp values. This type of document can likely be found online perhaps with the requirement of an API key.
