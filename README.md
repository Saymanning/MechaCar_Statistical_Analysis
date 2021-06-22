# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

The MechaCar_mpg.csv dataset was analyzed using R to create a linear regression model to answer the following questions:

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

- Is the slope of the linear model considered to be zero? Why or why not?

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?


The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. 

- **Question:** Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

   **Answer/Result:** "Vehicle_length" and "ground_clearance" were the variables provided a non-random amount of variance to the mpg values in the dataset.

- **Question:** Is the slope of the linear model considered to be zero? Why or why not?

   **Answer/Result:** No, the  slope of this linear model is not Zero becasue p-value of this model is 5.35e-11 which is less than 0.05.

- **Question:** Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

   **Answer/Result:** Yes, this linear model predicts the mpg of MechaCar prototypes effectively. The r-squared value of this model is 0.7149 which means approx. 71% of mpg    prediction is determined by this model.

<img width="904" alt="MPG 1" src="https://user-images.githubusercontent.com/78699465/122970299-b9f11000-d35b-11eb-8875-de7b1dd95074.png">
<img width="578" alt="MPG 2" src="https://user-images.githubusercontent.com/78699465/122970316-be1d2d80-d35b-11eb-8ee6-1e915607203c.png">
<img width="485" alt="MPG 3" src="https://user-images.githubusercontent.com/78699465/122970326-c1181e00-d35b-11eb-9c24-95ab25f9508e.png">


## Summary Statistics on Suspension Coils

The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. The summary statistics seen below were created using R to display the suspension coil's PSI continuous variable across all manufacturing lots and the PSI metrics for each lot.

- **Question:** The design specifications for the MechaCar suspension coils require that the variance of the suspension coils not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

   **Answer/Result:** As shown in the tables below,  the current manufacturing data does meet the criteria for all the lots in total as the variance is 62.29. Lots 1 and 2 meet the specifications with variances of 0.98 and 7.47. Lot 3 has a variance of 170.29 which exceeds the maximum of 100 pounds per square inch.
<img width="458" alt="lot_summary" src="https://user-images.githubusercontent.com/78699465/122970657-2d931d00-d35c-11eb-9f3b-3232b9a517ce.png">
<img width="376" alt="total_summary" src="https://user-images.githubusercontent.com/78699465/122970681-3388fe00-d35c-11eb-9cf0-0a7ce5536f30.png">


## T-Tests on Suspension Coils

For the next section of the analysis, t-tests were performed to determine if all manufacturing lots and each lot individually was statistically different from the population mean of 1,500 pounds per square inch. As seen in the images below, lot 1 and lot 2 have similar to the sample estimates mean 1500 however lot 3 is less than the sample estimates mean.

T-test lot 1: p-value of 1

<img width="508" alt="ttest 1" src="https://user-images.githubusercontent.com/78699465/122974367-3685ed80-d360-11eb-807c-00ef08dbe34a.png">

T-test lot 2:p-value of 0.61

<img width="557" alt="ttest 2" src="https://user-images.githubusercontent.com/78699465/122973246-05f18400-d35f-11eb-84d2-95030b675068.png">

T-test lot 3:p-value of 0.04

<img width="560" alt="ttest 3" src="https://user-images.githubusercontent.com/78699465/122974400-40a7ec00-d360-11eb-9bfe-0d13483cb51a.png">

T-test all lots

<img width="513" alt="ttest all" src="https://user-images.githubusercontent.com/78699465/122973261-0b4ece80-d35f-11eb-8af7-1c6f4b4b0e49.png">



## Study Design: MechaCar vs Competition

- **What metric or metrics are you going to test?**: Safety - Does MechaCar produce a safer vehicle than the competition?
  The metrics used would be safety ratings of MechaCar and other car  manufacturers.
  
- **What is the null hypothesis or alternative hypothesis?**: There is no statistical difference between MechaCar and their competition in terms of cost and safety ratings. An alternative hypothesis would be that MechaCar does not have statistically significant higher safety ratings than vehicles from other manufacturers. 

- **What statistical test would you use to test the hypothesis?**: Multiple Linear Regression and T-tests.

- **What data is needed to run the statistical test?**: Safety ratings data from MechaCar as well as  the competition's safety ratings data.
