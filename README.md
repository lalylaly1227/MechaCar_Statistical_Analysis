# MechaCar_Statistical_Analysis

## Deliverable 1: Linear Regression to Predict MPG
> Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

* The vehicle length, and vehicle ground clearance are statistically likely to provide non-random amounts of variance to the model. The vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Equally, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-values that indicate a random amount of variance with the dataset.

> Is the slope of the linear model considered to be zero? Why or why not?

* The p-Value for this model, is much smaller than the assumed significance level of 0.05%. This indicates there is sufficient evidence to reject our null hypothesis, which further indicates that the slope of this linear model is not zero.

> Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

* This linear model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model. In this scenario, the multiple regression model does predict mpg of MechaCar prototypes effectively.

## Deliverable 2: Create Visualizations for the Trip Analysis
> The suspension coil’s PSI continuous variable across all manufacturing lots
<img width="481" alt="total_summary" src="https://user-images.githubusercontent.com/105124485/189449897-64e85dcc-056a-4930-b81f-f479aed8d4a6.png">

> The following PSI metrics for each lot: mean, median, variance, and standard deviation
<img width="638" alt="lot_summary" src="https://user-images.githubusercontent.com/105124485/189449888-bfc990c3-5f17-46d1-9019-0116966c5371.png">

Lot 1 and Lot 2 are almost identical and fall within the design specifications. Lot 3 has the most variance and exceeds the manufacturers specs.
<img width="967" alt="plt2" src="https://user-images.githubusercontent.com/105124485/189450295-201f1e41-729a-458f-ae07-40c3bf189ecf.png">


In the total summary, the variance of all three lots does fall under the maximum variance of 100 PSI with a variance of 62 PSI.

In the lot summary, the major contributor to the variance is lot 3 with a variance of 170 PSI with the other two lots having variances of less than 8 PSI.


In total, the manufacturing data meets the maximum variance in PSI requirement, but there are clearly big problems in lot 3 with a variance of 170 PSI. Lot 3 does not meet the maximum variance requirement.

## Deliverable 3: T-Tests on Suspension Coils
The summary demonstrates that the true mean of the sample is 1498.78, there is not enough evidence to support rejecting the null hypothesis. The mean of all three manufacturing lots is statistically like the presumed population mean of 1500.

<img width="467" alt="mecha_coil Sample t-test" src="https://user-images.githubusercontent.com/105124485/189450095-bd456a9b-5a3c-4a09-864d-d0a7edd06c6c.png">

If we look at the individual lots, Lot 1 sample has the true sample mean of 1500, again as we saw in the summary statistics above. With a p-Value of 1, we cannot reject the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean of 1500.
<img width="457" alt="Lot1 Sample t-test" src="https://user-images.githubusercontent.com/105124485/189450055-0be21cb1-4f89-4d36-863a-105ddfbdf87d.png">

Lot 2 has essentially the same outcome with a sample mean of 1500.02, a p-Value of 0.61; the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.
<img width="418" alt="Lot2 Sample t-test" src="https://user-images.githubusercontent.com/105124485/189450066-1d0bbbf0-c30a-4961-ba44-ca04da24133a.png">

But, Lot 3, is a different situation. Here the sample mean is 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05. All indicating to reject the null hypothesis that this sample mean and the presumed population mean are not statistically different. Something went amiss in Lot 3's production cycle. The process needs to be checked for system fails and the suspension coils from this lot need to be inspected to remove those not meeting quality criteria.

<img width="420" alt="Lot3 Sample t-test" src="https://user-images.githubusercontent.com/105124485/189450080-c32f0b23-b9b1-4009-8242-b123e2302d3b.png">

## Deliverable 4: Design a Study Comparing the MechaCar to the Competition
There are many features that consumers look at when purchasing a car, among them are the price of the vehicle, MPG, luxury features such as leather seating, etc.

> What metric or metrics are you going to test?

* Metrics to be tested:

•	Current Selling Price  
•	Engine Type (Electric, Hybrid, Gasoline) 
•	Holds its Value
•	Safety Features
•	Maintenance Package
•	MPG (Gasoline Efficiency)

> Hypothesis: Null and Alternative

*First, we will determining which factors are key for the MechaCar's genre:

• Null Hypothesis: MechaCar is priced correctly based on its performance of key factors for its genre.
• Alternative Hypothesis: MechaCar is not priced correctly based on performance of key factors for its genre.

> What statistical test would you use to test the hypothesis? And why?

* I recommend using the t-test to compare the new dataset with the market competitors. The t-test has proven to be a good analysis tool and provided the predictions needed to take the next steps for improvement in our current challenge.

What data is needed to run the statistical test?

All data is to be numerical; 	Data samples will be as large as possible; Data samples need to be randomly selected; Variance of data needs to be similar.
