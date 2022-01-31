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
