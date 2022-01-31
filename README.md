# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

#### Multiple Linear Regression 

![image](https://user-images.githubusercontent.com/89496798/151726874-d93fd8c2-1dca-4b8d-815b-b83d14c7d237.png)

#### Summary Statistics       

![image](https://user-images.githubusercontent.com/89496798/151726858-7c160b06-fac6-4bd3-95b4-3af985a09807.png)

##### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
The variables/coefficients that provide a non-random amount of variance to the mpg values in the dataset are the vehicle length, ground clearance, and the intercept.

##### Is the slope of the linear model considered to be zero? Why or why not?
Per our summary statistics shown above, our p-value for the given linear gregression model is 5.35 x 10^-11, which is smaller than our assumed significance level of 0.05%, We can state that there's sufficient evidence to reject our null hypothesis - this tells us the slope of our linear model is **not zero**.

##### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
We can refer to the r-value from our analysis to help determine if the linear model effectively predicts the mpg of MechaCar prototypes. As our Multiple R-squared value is 0.7149 (71.49%), we can consider our linear model shows a strong correlation between the MechaCar data and mpg.

## Summary Statistics on Suspension Coils

### Total Summary
![image](https://user-images.githubusercontent.com/89496798/151728602-232b10a4-3309-442e-952f-956288647206.png)

### Lot Summary

![image](https://user-images.githubusercontent.com/89496798/151728618-253022e4-148a-4976-a613-818656eae3c0.png)

#### The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

The design specifications for the MechaCar suspension coils accurately dictate that the variance of all suspension coils must not exceed 100 pounds per square inch for all manufacturing lots with a variance of 62.29 given our Total_Summary dataframe shown above. Per our Lot_Summary summary statistics, it appears Lot 1 and 2 do not exceed 100 pounds per square inch with variances of 0.98 and 7.47. However, Lot 3 does exceed 100 pounds per square inch with a variance of 170.29.


## T-Test on Suspension Coils

### Summary T-Test on all Manufacturing Lots

![image](https://user-images.githubusercontent.com/89496798/151729583-713fa62f-904c-4411-821a-e6ee8cf2ed7b.png)

#### Statistical Significance of Population Mean
Given our T-Test on all manufacturing lots, our t-value is -1.8931 and our sample mean is 1498.78. With our p-value of 0.06028 being greater than the common significance level of 0.05, we don't have sufficient evidence to reject the null hypothesis and we can determine that the two means are statistically similar. We can break this down further by running t-tests on all individual manufacturing lots.

## Summary T-Test on Lots 1, 2, and 3

### Lot 1

![image](https://user-images.githubusercontent.com/89496798/151730682-7ad5ca18-2489-440b-8d62-3a66fc991e49.png)

#### Statistical Significance of Population Mean From Lot 1
As for our T-Test of Lot 1, our t-value is 0 and our sample mean is 1500. With our p-value of 1 being greater than the common significance level of 0.05, we don't have sufficient evidence to reject the null hypothesis and we can determine that the two means are statistically similar.

### Lot 2

![image](https://user-images.githubusercontent.com/89496798/151730709-f5d9352a-525b-40b2-b4c4-d2d37e261796.png)

#### Statistical Significance of Population Mean From Lot 2
For our T-Test of Lot 2, our t-value is 0.51745 and our sample mean is 1500.2. With our p-value of 0.6072 being greater than the common significance level of 0.05, we don't have sufficient evidence to reject the null hypothesis and we can determine that the two means are statistically similar.

### Lot 3

![image](https://user-images.githubusercontent.com/89496798/151730741-8f91675d-2f69-4b6b-b3cf-1699d07d4acc.png)

#### Statistical Significance of Population Mean From Lot 3
Finally for our T-Test of Lot 3, our t-value is -2.0916 and our sample mean is 1496.14. With our p-value of 0.04168 being **less** than the common significance level of 0.05, we **do have** sufficient evidence to reject the null hypothesis and we can determine that the two means **are not** statistically similar.

## Study Design: MechaCar vs Competition

### What metric or metrics are you going to test?
- Fuel economy
- Type of vehicle/motor (gasoline, electric, hybrid)
- Availability
- Depreciation/resale value
- Average vehicle life span

### What is the null hypothesis or alternative hypothesis?
- Null Hypothesis - The type of vehicle/motor does not significantly impact the fuel economy, availability, depreciation/resale value, or average life span.
- Alternative Hypthesis - The type of vehicle/motor does significantly impact the fuel economy, availability, depreciation/resale value, or average life span.

### What statistical test would you use to test the hypothesis? And why?
- To statistically test these metrics, we may also use a multiple linear regression to help determine the statistical difference between the type of vehicle/motor and its fuel economy, availability, depreciation/resale value, and average life span. For example. an electric protoype may show better fuel economy but can also affect the availability of the vehicle. A more specific example of its potential competition would be Tesla's electric vehicles. With eletric vehicles having excellent fuel economy and a long life-span, the demand for the vehicle significantly surpasses that of the supply.

### What data is needed to run the statistical test?
- Numerical data may be needed in regards to the car's fuel economy (miles per gallon) and also nominal data related to the type of vehicle/motor.
