# MechaCar_Statistical_Analysis

### Linear Regression to Predict MPG
Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

<!---![Results](https://github.com/sag7221/MechaCar_Statistical_Analysis/blob/main/visualizations/One_Sample_test_Entire_PSI_Column.png)-->
<img src="https://github.com/sag7221/MechaCar_Statistical_Analysis/blob/main/visualizations/One_Sample_test_Entire_PSI_Column.png" width="550">

Here looking at the summary results, the variables : vehicle_length, ground clearance and Intercept provide the least variance and are absolutely needed to determine and predict the mpg.

Is the slope of the linear model considered to be zero? Why or why not?
The slope of the linear model is not zero. Had it been zero, there would be no variables providing significance to the prediction of mpg.
But in this case, we see that there are some variables which provide a huge signoficance in determining the mpg.

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
Yes, this linear model does predict mpg of MechaCar effectively. This can be derived from the result of R-squared, 0.7149 (71.4% of times, it can predict the mpg correctly)

### Summary Statistics on Suspension Coils
So for this I have created 2 visualizations. \
\
Visualization 1: Mean, Median, Variance and Std Deviation for the PSI column on the whole.

<img src="https://github.com/sag7221/MechaCar_Statistical_Analysis/blob/main/visualizations/summarize_info_PSI.png" width="550">

Visualization 2: Mean, Median, Variance and Std Deviation of the pSI for each manufacturing lot type.
<img src="https://github.com/sag7221/MechaCar_Statistical_Analysis/blob/main/visualizations/lot_summary_PSI.png" width="550">



Question: The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

Answer: After going through the results, i can say that variance for PSI column on the whole does not exceed 100 pounds per square inch.
Manufacturing data does meet this design specification.
Now looking at PSi values for each Mnaufacturing Lot. Here we can conclude that Variance for Lot 3 is 170 which is more than the maximum threshold of 100 PSI.
Hence Lot 3 fails the test.
Lot 1 and Lot 2 meet the design specificiation.

### T-Test on Suspension Coils

Here i carried out One sample t-tests. The results are as follows.

#### T-Test on combined Lots
One sample test on combined lots.

<img src="https://github.com/sag7221/MechaCar_Statistical_Analysis/blob/main/visualizations/One_Sample_test_Entire_PSI_Column.png" width="550">

Here, the p-value of t-test is much greater than 0.05, hence we cannot reject the null hypothesis. Mean of combined lots is statistically similar to the population mean of 1500

#### T-Test on Lot1

<img src="https://github.com/sag7221/MechaCar_Statistical_Analysis/blob/main/visualizations/t_test_lot1.png" width="650">

Here the p-value is 1 so we cannot reject the null hypothesis as the value is much greater than 0.05. Mean of Lot1 is also statistically simialr to population mean of 1500

#### T-Test on Lot2

<img src="https://github.com/sag7221/MechaCar_Statistical_Analysis/blob/main/visualizations/t_test_lot2.png" width="650">

p-value here is 0.6072 which is still greater than 0.05 and we cannot reject the null hypotheses here as well. Mean of Lot2 is also statistically similar to population mean of 1500


#### T-Test on Lot3

<img src="https://github.com/sag7221/MechaCar_Statistical_Analysis/blob/main/visualizations/t_test_lot3.png" width="650">

p-value here is 0.04 which is lesser than 0.05 and hence we can reject the null hypothesis. Here as the null hypothesis can be rejected, the mean of lot3 is NOT statistically similar to the population mean of 1500.

