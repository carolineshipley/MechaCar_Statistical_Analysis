# MechaCar_Statistical_Analysis

## Project Overview

The purpose of this project is to analyze metrics that can affect the manufacturing of MechaCar, a car prototype, and compare vehicle performance across different manufacturer lots. The metrics analyzed include vehicle length, weight, spoiler angle, ground clearance, AWD, MPG, and PSI.

## Linear Regression to Predict MPG

For this analysis was performed multiple linear regression to see if it could predict MPG dependent variable by using the vehicle length, weight, spoiler angle, ground clearance, and AWD independent variables. This analysis aims to answer these three questions:

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
2. Is the slope of the linear model considered to be zero? Why or why not?
3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

### Analysis Results:

![Linear Regression](https://github.com/carolineshipley/MechaCar_Statistical_Analysis/blob/main/Resources/linear_regression_summary.PNG)

### Analysis Conclusion

1. Two variables provided a non-random amount of variance, the vehicle length and ground clearance. Both have extremely small p-value meaning that they had a high level of significance. It's also important to note that the intercept have a high level of significance, so there are still other factors contributing to the variance of the MPG of the MechaCar.
2. The linear regression shows that some of the independent variables had a significant effect on the dependent variable. If none of the independent variables had an effect on the dependent variable then the linear regression would be a zero slope. With that said the slope of the linear model is not considered to be zero.
3. Multiple R-squared increases as more variables are passed through the regression. However, adjusted R-squared controls against this increase, making it a more accurate predictor of how effective the linear model is. An adjusted R-square of 0.6825 shows that this linear model predicts the MPG of MechaCar relatively well.


## Summary Statistics on Suspension Coils

The overall variance for the entire dataset shows that the current manufacturing data meets the 100 pounds per square inch variance limitation. However, when the lots are analyzed separated, the third lot demonstrates a much higher variance exceeding the 100 pounds per square inch variance limitation.

![total_summary_table](https://github.com/carolineshipley/MechaCar_Statistical_Analysis/blob/main/Resources/total_summary_table.PNG)
![lot_summary_table](https://github.com/carolineshipley/MechaCar_Statistical_Analysis/blob/main/Resources/lot_summary_table.PNG)

## T-Test on Suspension Coils

### T-Test on Entire Lot

![t_test](https://github.com/carolineshipley/MechaCar_Statistical_Analysis/blob/main/Resources/t_test.PNG)

At a significance level of 0.05, we fail to reject the null hypothesis since the p-value equals 0.06. Therefore, we cannot reject the fact that the sample mean may be equivalent to the population mean. 



### T-Test on Three Lots

![lots_t_test](https://github.com/carolineshipley/MechaCar_Statistical_Analysis/blob/main/Resources/lots_t_test.PNG)

#### Lot 1
At a significance level of 0.05, we fail to reject the null hypothesis since the p-value equals 1. Therefore, we cannot reject the fact that the sample mean may be equivalent to the population mean. 

#### Lot 2
At a significance level of 0.05, we fail to reject the null hypthesis again since the p-value equals 0.6072. Therefore, we cannot reject the fact that the sample mean may be equivalent to the population mean. 

#### Lot 3
At a significance level of 0.05, we can reject the null hypothesis since the p-value equals 0.04168. Therefore, we can reject the fact that the sample mean may be equivalent to the population mean. 


## Study Design: MechaCar vs. Competition
Another statistical analysis that can be performed to determine MechaCar's performance compared to its competition is a linear regression on city and highway fuel efficiency. With gasoline prices rising and the consumers concern with environmental impact increasing, it is an important feature that many consumers look at when purchasing a new car. This is the proposed study design:

1. The metrics to test are city and highway fuel efficiencies.
2. The Null Hypothesis is that all of the cars in the same class have the same fuel efficienies. The Alternative Hypothesis is that they are not all the same.
3. Taking into consideration 5 car class types, the statystical test used on this study would be ANOVA for both types of fuel efficiencies. ANOVA is more indicated than t-test for statistical tests with three or more variables.
4. The data used for the statistical test would be fuel efficiency data from 100 cars per class type to create a sample size of data.
