**SENG 438- Software Testing, Reliability, and Quality**

**Lab. Report \#5 – Software Reliability Assessment**

| Group \#: 18     |     
| -------------- |
| Student Names: |     
|Abdul Rafay        |    
|Mohammed Azmath Khan|
|Taiwu Chen           |     
|Hashir Naved         | 

# Introduction
The objective of this lab was to analyze integration test data using reliability assessment tools. The two methods that were implemented in order to assess the failure data were reliability growth testing and reliability demonstration charts (RDC) for the reliability assessment. This lab also provides the opportunity to compare different reliability assessments to inspect the pros and cons of each and improve future decisions on tool usage.



# Assessment Using Reliability Growth Testing
## Result of model comparison (selecting top two models)
Using the C-SFRAT tool, we were able to plot all the models and covariates and analyze the trend between the plotted data. The models selected include:

- IFR Salvia and Bollinger
- S Distribution
- Discrete Weibull (Order 2)
- IFR Generalized Salvia and Bollinger
- Negative Binomial (Order 2)
- Geometric
- Truncated Logistic

hen finding the best two models, C-SFRAT made it easy to compare the different models using the model comparison tab which allowed us to see which one would fit the best into our failure data. We used the Log-Likelihood to determine which fit best as it is used as a way to measure the goodness of fit for a model.
![Caption 1](media/1.png)  
Figure 1 - Two best models (S on E,F,C) and (NB2 on E,F,C)

## Result of range analysis (an explanation of which part of data is good for proceeding with the analysis)
We decided to use all of the range because:
- A good model fit appears along the entire duration which suggests that collected data conforms to projected reliability growth trends.
- This data interval shows no indications of problems or disturbances that should warrant removing any sections.
- The inclusion of this entire dataset ensures maximum data availability which produces statistics-based reliable estimations of reliability growth parameters.
- The range extends through the entire test time from start to finish abecause it demonstrates the entire pattern of reliability growth for the system.

## Plots for failure rate and reliability of the SUT for the test data provided
![Caption 2](media/2.png)  
Figure 2 - MVF Graph

![Caption 3](media/3.png)  
Figure 3 - Failure Intensity Graph

![Caption 4](media/4.png)  
Figure 4 - Reliability Graph Prediction

## A discussion on decision making given a target failure rate
![Caption 4](media/5.png)  
Figure 5 - Failure Intensity Graph With 0.1 Target Failure Intensity
For deciding on the failure rate target we used the C-SFRAT tool again to help us predict the testing of the new prediction intervals. We were able to make a target the failure rate being which is dividing the failure numbers by the total number of hours the system is running. Failure rate also helps us in determining how much we need to improve our testing in order to bring this rate down in order to gain assurance on the number of failures the system would experience when released to the end-users. Our aim was to have the lowest possible rate we could to ensure the reliability of the failure data given to us is not at a dangerous level in terms of the safety of the application. With our two predictions, we wanted to set a target of the failure rate to be 0.1 as this was the lowest intensity for both of the models in the desired intervals for the intensity graph displayed in the above section. With this target failure rate, the failure data shall provide reliability to the system under the testing where this data originated from.

 ## A discussion on the advantages and disadvantages of reliability growth analysis

Advantages:
- Reliability Growth Testing produces visualized graphs that shows the failure rates (relationship between failure to time intervals), which are important when developing a product.
- RTG is also used to predict the data behaviour in the future to provide us information for making decisions on the product. Specifically, we can use the average failure rates in a range of intervals to calculate the System Reliabilty which is used to identify the remaining bugs and remaining time that is needed to remove the excessive bugs.
- RTG allows us to backtrack the causes of system failures by identifying the highest failure peaks.
Disavantages:
- It depends on large number of fail cases in order to be accurate.
- There can be a lot of noisy data when analyzing the inputs and drawing the graphs.
- The graphs are difficult to understand and need high-level knowledge in statistic and quality assurance to utilize it


# Assessment Using Reliability Demonstration Chart 

# 

# Comparison of Results

# Discussion on Similarity and Differences of the Two Techniques

# How the team work/effort was divided and managed

# 

# Difficulties encountered, challenges overcome, and lessons learned

# Comments/feedback on the lab itself
