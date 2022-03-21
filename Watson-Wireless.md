Introduction and Scope:
-----------------------------
Watson Wireless (WW) is a telecommunications firm serving regional markets in Brazil and Argentina. Recently WW has struggled with revenue contraction as customers move to other competitors. WW leadership has prioritized reducing customer churn in the next period. WW seeks answers to the following key questions:

1) What are the most important drivers of customer churn?
2) What are 2-3 recommendations for how WW can use this information to reduce customer churn in the future?

Our analysis process included the following steps:
------------------------------------------------------------
- Exploratory Data Analysis<br>
- Feature Selection: using cross tabulation, correlations, and SelectKBest feature selection model.<br>
- Modeling: we tried three models for this classification problem, namely, Logistic Regression, Support Vector Classifier and Random Forest Classifier. Logistic Regression produced the highest cross validation accuracy. The next step was fine tuning the model hyperparameters to improve the model performance.<br>
- Finally the tuned model was tested against the testing set to arrive the expected out of sample accuracy.

Conclusions and Recommendations
-------------------------------------------
Based on our analysis we provide the following conclusions and recommendations for the future:

The strongest three predictors affecting consumer retention (churn = 0) are as follows:<br>
- tenure<br>
- address<br>
- employ<br>

The strongest three predictors affecting consumer churn are as follows:<br>
- income<br>
- equip<br>
- age<br>

Observations:
-----------------
- Our model is better at predicting retention (churn = 0) than churn (churn = 1). This is due to the dataset containing more observations with churn=0 than churn=1. Our model should become better at predicting churn if the dataset is updated with more observations for +ve churn customers

- Customers in certain address code (range 0-11) have a high churn percentage. This could be due to network issues in theses areas. Futher investigation is advised

- Customers in low income range (0-47) are more likely to leave WW. Further analysis is advised on price plans for these customers

- Customers who have equip = 1 are more likely to leave WW. Futher analysis advised to uncover reasons for this

- Customers with high years of education and employment are more loyal. Should proivde more incentives to attract these types of customers
