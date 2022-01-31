# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

#### Multiple Linear Regression 

Call:
lm(formula = mpg ~ vehicle_length + vehicle_weight + spoiler_angle + 
    ground_clearance + AWD, data = MechaCar_table)

Coefficients:
     (Intercept)    vehicle_length    vehicle_weight     spoiler_angle  ground_clearance               AWD  
      -1.040e+02         6.267e+00         1.245e-03         6.877e-02         3.546e+00        -3.411e+00 
       
#### Summary Statistics       

Call:
lm(formula = mpg ~ vehicle_length + vehicle_weight + spoiler_angle + 
    ground_clearance + AWD, data = MechaCar_table)

Residuals:
     Min       1Q   Median       3Q      Max 
-19.4701  -4.4994  -0.0692   5.4433  18.5849 

Coefficients:
                   Estimate Std. Error t value Pr(>|t|)    
(Intercept)      -1.040e+02  1.585e+01  -6.559 5.08e-08 ***
vehicle_length    6.267e+00  6.553e-01   9.563 2.60e-12 ***
vehicle_weight    1.245e-03  6.890e-04   1.807   0.0776 .  
spoiler_angle     6.877e-02  6.653e-02   1.034   0.3069    
ground_clearance  3.546e+00  5.412e-01   6.551 5.21e-08 ***
AWD              -3.411e+00  2.535e+00  -1.346   0.1852    
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

Residual standard error: 8.774 on 44 degrees of freedom
Multiple R-squared:  0.7149,	Adjusted R-squared:  0.6825 
F-statistic: 22.07 on 5 and 44 DF,  p-value: 5.35e-11

### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
The variables/coefficients that provide a non-random amount of variance to the mpg values in the dataset are the vehicle length, ground clearance, and the intercept.

### Is the slope of the linear model considered to be zero? Why or why not?
Per our summary statistics shown above, our p-value for the given linear gregression model is 5.35 x 10^-11, which is smaller than our assumed significance level of 0.05%, We can state that there's sufficient evidence to reject our null hypothesis - this tells us the slope of our linear model is **not zero**.

### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
We can refer to the r-value from our analysis to help determine if the linear model effectively predicts the mpg of MechaCar prototypes. As our Multiple R-squared value is 0.7149 (71.49%), we can consider our linear model shows a strong correlation between the MechaCar data and mpg.
