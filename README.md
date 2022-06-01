# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. 
### Statistical Study
#### Metrics collected for each vehicle
* vehicle length
* vehicle weight
* poiler angle
* drivetrain
* ground clearance
#### Design 
Designed a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file. 
#### Results

![image](https://user-images.githubusercontent.com/96931376/171300662-27988a75-4e1e-44b1-8d17-7df6fc959912.png)
##### Above output shows the following:
1. For MechaCar prototype, vehicle length and vehicle ground clearance are statistically likely to correlate with miles per gallon. 
2. These variables reflected a random amount of variance within this dataset: 
* vehicle weight
* spoiler angle
* All Wheel Drive (AWD)
##### Linear 
1. The p-Value is significantly smaller than the assumed significance level of 0.05%
2. There is sufficient evidence to reject our null hypothesis
3. Slope of this linear model is not likely to be zero
4. Approximately 71% of all mpg predictions will be determined by this model
5. Multiple regression model does predict mpg of MechaCar prototypes effectively

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.
### Results
* MechaCar suspension coils mandate that the variance of the suspension coils cannot exceed 100 pounds per square inch (PSI)
* Variance of the coils entireWhen looking at the entire population of the production lot, the variance of the coils is 62.29 PSI, which is well within the 100 PSI variance requirement
* Lot 1 and Lot 2 are meet the mandated design specifications; however, Lot 3 shows a large variance in performance and consistency
* Lot 3  is disproportionately causing the variance at the full lot level
This very simple boxplot illustrates the differences between the lots:

![image](https://user-images.githubusercontent.com/96931376/171301833-f148c665-7927-49cc-bf17-5fa235f6c1b4.png)

## T-Tests on Suspension Coils
T-tests performed to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch. The mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.
Summary of the t-test results across all manufacturing lots: 

![image](https://user-images.githubusercontent.com/96931376/171302550-286c1cdd-ed46-429d-b93d-3471c0ef4887.png)
* Lot 1 
  * True sample mean of 1500
  * p-Value of 1
  * No statistical difference between the observed sample mean and the presumed population mean (1500)
* Lot 2
  * Sample mean of 1500.02
  * p-Value of 0.61
  * Statistically similar between the sample mean and the population mean of 1500
* Lot 3
  * Sample mean is 1496.14
  * p-Value is 0.04 (lower than the common significance level of 0.05)
  * Lot 3 statistically indicates the rejection of the null hypothesis as this sample mean and the presumed population mean are     not statistically different
 
![image](https://user-images.githubusercontent.com/96931376/171303146-00483e38-faa8-4150-8b80-f99b29f59dd4.png)

## Study Design: MechaCar vs Competition
Design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturer. 
### Statistical Study
#### Design
* Defined the metric to be tested
* Determined the null hypothesis or an alternative hypothesis
* Described the statistical test for the hypothesis
* Collected data on MechaCar and it's comparable models across several different manufacturers over a defined duration
#### Metrics
* Safety Feature Rating: Independent Variable
* Current Price (Selling): Dependent Variable
* Drive Package : Independent Variable
* Engine (Electric, Hybrid, Gasoline / Conventional): Independent Variable
* Resale Value: Independent Variable
* Average Annual Cost of ownership (Maintenance): Independent Variable
* MPG (Gasoline Efficiency): Independent Variable
#### Hypothesis: Null and Alternative
* Null Hypothesis (Ho): MechaCar is priced correctly based on its performance of key factors for its genre.
* Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance of key factors for its genre.
#### Statistical Tests
Used a multiple linear regression to determine the factors that have the highest correlation to predict the dependent variable (i.e., list selling price). This can be applied to determine the combination that has the greatest impact on price.
