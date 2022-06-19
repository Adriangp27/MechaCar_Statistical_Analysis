# MechaCar_Statistical_Analysis


## Linear Regression to Predict MPG
The mpg of MechaCar prototypes can be predicted using linear model derived from several factors which includes vehicle length, weight, spoiler angle, drivetrain, and ground clearance. After reading the csv file, I located the linear regresson function using the lm() function, and I calculated the summary statistics using the summary() function.


Following is the analysis produced by the script:

 - Variables "vehicle_length" and "ground_clearance" contributed a non-random amount of variance to the mpg values in the dataset.
 - As a result, the p-value (5.35e-11) is significantly lower than a significance level of 0.01. Because the statistical analysis provides sufficient evidence that the null hypothesis cannot be accepted, the slope of the linear model is considered to be non-zero.
 - MechaCar prototypes are predicted effectively by a linear model as their r squared value is 0.7149. Therefore, there is a reasonable chance that future data will also fit this model.

## Suspension Coils: Summary Statistics
With the suspension coil data, I generated a summary statistics table showing PSI continuous variable across all manufacturing lot, as well as PSI metrics for each lot. First, I read the CSV file and created a summary table for all manufacturing lots (the total_summary table). Next, I grouped the table based on the manufacturing lot to get the table for each manufacturing lot(the lot_summary table).

Tables produced by the scripts are as follows:

It was required that the MechaCar suspension coils had variances of no more than 100 pounds per square inch to meet the design specifications. Since the variance of all the lots is 62.29, the current manufacturing data meets the criteria. The variance of Lots 1 and 2 are both within the specification ranges of 0.98 g/cm2 and 7.47 g/cm2 respectively, but the variance for Lot 3 is 170.29 g/cm2 which is exceeding the maximum of 100 g/cm2.

## T-Tests on Suspension Coils
For each manufacturing lot and each individual lot, I conducted t-tests to see if they differed from the mean 1,500 pounds per square inch for the population.

Based on the script, the following analysis was produced:

All Lots of Manufacturing T-Test

According to the results of the t-test, there is enough evidence to reject the null hypothesis for all manufacturing lots with a p-value of 0.06. Therefore, the mean PSI of all manufacturing lots is statistically different from that of the population, which is 1,500 pounds per square inch.

Lot 1 T-Test

The PSI of Lot 1 was not statistically different from 1,500 pounds per square inch given the t-test p-value of 1. Therefore, the population PSI of Lot 1 is not statistically different from the Lot 1 PSI.

Lot 2 T-Test

In Lot 2, the t-test had a p-value of 0.61, indicating insufficient evidence to reject the null hypothesis. FOr this reason, the mean PSI of Lot 2 is statistically different from the mean PSI of the population of 1,500 pounds per square inch.

Lot 3 T-Test

Based on the positive t-test for Lot 3, there is enough evidence to reject the null hypothesis. Therefore, the mean PSI of Lot 3 is statistically different from the population mean of 1,500 pounds per square inch.

## Study Design: MechaCar vs Competition
A consumer's safety rating is one of the most important factors in choosing a new car. The safety rating of MechaCar vehicles will need to be compared to other manufacturers' ratings by means of a statistical study. There is no statistical significant difference between MechaCar and the othe manufacturers' safety ratings, while the alternative hypothesis is that MechaCar does have statistical significant higher safety ratings than that if vehicles from other manufacturers. One way to determine if there is any difference between the groups would be to run a one-tailed t-test. Because we know the direction of the difference, we wouldn't use a two-tailed t-test. MechaCar vehicles and their respective safety ratings, along with the scores of cars from a variety of other manufacturers, are the data needed to run the statistical test.