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

The design specifications for the MechaCar suspension coils accurately dictate that the variance of all suspension coils must not exceed 100 pounds per square inch for all manufacturing lots given our Total_Summary dataframe shown above. Per our Lot_Summary summary statistics, it appears Lot 1 and 2 do not exceed 100 pounds per square inch with variances of 0.98 and 7.47. However, Lot 3 does exceed 100 pounds per square inch with a variance of 170.29.
