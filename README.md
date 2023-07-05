## Central Limit Theorem for Process Improvement with Python 📊
*Estimate the workload for reverse logistics.*


Returns management is often something I deal with a lot. 
 
Usually it consists of receiving goods, sorting, organizing, and inspecting their quality.
 
What I would like to go through is a challenge of estimating the workload ahead for processing returns.
 
Luckily, we have the Central Limit Theorem for this.
 
Crudely stated, if you have a sufficiently large sample from a population, the sample mean tends to be normally distributed, even if the population isn’t normally distributed.
 
This is a hack of nature which helps us because a normal distribution is where:
> The mean, median and mode are the same.
> The distribution is symmetric about the mean (half the values fall below the mean and half above the mean)
> The distribution can be described by two values: Mean and Standard Deviation.
> Around 68% of values are within 1 standard deviation from the mean.
> Around 95% of values are within 2 standard deviations from the mean.
> Around 99.7% of values are within 3 standard deviations from the mean.
 
Hypothetical Problem
As Inbound Reverse Logistics come in, what is the estimate that we will have 30 items per carton?
 
I know the productivity of handling one item and I would like to estimate the workload in hours based on the number of cases I will receive in the week. 
 
Based on the historical data, I know:
Mean of 23 items per carton
Standard deviation of 7 items
 
My team is usually sized to handle a maximum of 30 items per case. 
 
I need to hire temporary workers to meet the daily capacity target if it goes beyond this threshold.
 
Action
First, I would need to estimate my distribution. I know that the historical data of the total population has a mean µ = 23 items per carton and a standard deviation of σ = 7 items per carton.
 
Second, I randomly measure a number of items per carton (x) using n samples.
 
z = (x – μ) / σ
 
Third, I take the assumption that my observations are independent and identical and that returns are coming from all customers.
 
Fourth, I calculate the normal distribution based on the data obtained. 
 
Code can be found in the comments below.
 
From the distribution I can tell that if I size the team based on 35 items per carton, I will have adequate workforce for 95% of all returns.
 
This means adding temporary staff for the extra 5 items per carton.
 
This is the power of the central limit theorem in supply chain analytics.


## Code
This repository code you will find all the code used to explain the concepts presented in the article.

## About me 🤓
Supply Chain Professional with international experience and a passion for data science. \
Connect with me on LinkedIn: [Profile](https://www.linkedin.com/in/victorkharvey/)
Read my supply chain portfolio: [Portfolio](https://www.linkedin.com/pulse/repository-writing-code-victor-harvey/)
