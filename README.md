# Exploratory Data Analysis
## By Caleb Denzeil

# Dataset 1(Churn_Modelling.csv)
> The first dataset contains information about whether the bank customers or subscribers will discontinue a service or not
 and it's depicted as (1=yes or 0=no)
 
 # Dataset 2(insurance.csv)
 > The second dataset contains information about health insurance charges.A person is offered insurance depending on a number of factors like age, bmi or if the person is a smkoker or non-smoker.
 > I did some feature engineering and divided the age and bmi columns into different categories
 
 ## Summary of Findings(Dataset 1)
 
> Their is no relationship between age and Creditscore.

> Germany has the highest credit score

> 7962 customers remained and 2037 customers exited. That's 79.63% and 20.37% of customers.

> More female customers have exited than males.

> Their is a weak relationship between Tenure and creditscore. Customers with higher credit score have more tenures

> Their is a weak relationship between EstimatedSalary and Age. Younger customers have a higher Estimated salary compared to the older generation

> After doing exploratory data analysis, I trained the dataset using an ensemble model, Random forest with bootstrapping.The model was supposed to predict how many customers would leave the bank or stay.

>The independent variables that I used were 'CreditScore', 'Age', 'Tenure', 'Number_of_Products', 'Has_credit_card', 'IsActiveMember' and the dependent variable was Exited

>The model  predicted correctly 82% of the cases. 

>After doing the first prediction, I trained the model with different number of estimators and 90 produced a model with highest accuracy score of 84.13% which is better than the previous one.
 
## Summary of Findings(Dataset 2)


> A majority of the smokers belong to the old_adults bracket and the young_adults are the least.

> Their is not that much of a relationship between age and bmi because their is a slight difference in their mean,older adults have a higher bmi compared to young adults.

> Females and males have almost the same bmi, although the male's bmi is higher seconded by females.

> The old adults are charged the most and the young adults the least.

> People with a higher bmi are charged more compared to those with less.

> Both smokers and non-smokers have almost the same bmi.

>I applied a gradient boosting algorithm to do predictive analysis. My independent variable was bmi and dependant charges.

>The model did not perform well with an accuracy of 0.07 on the test set and 0.02 on the training data.The model was not fit for the predictive analysis. 