Introduction
------------
Globex is a large industrial company with presence in six continents. They produce large industrial products such as ships, power plants, engines, etc. The CFO is examining profitability for numerous projects around the world, starting with projects beginning in 2010. They believe that using data and analytics can help identify projects that may be risky and result in a loss of profit. Globex has compiled data on all completed projects with a start date of 2010 or later.

Globex needs the following:
- Determine the key predictors of a project’s “PROFIT_PLAN”.
- Develop an actionable, innovative strategy for the client.
- Prepare a deliverable that is clear and concise, outlining each of your key recommendations.


Process
-------
Our process included the following steps:
- Exploratory Data Analysis: to look at information about our dataset and the variables in it in order to get a flavor of its different aspects.
- Feature Selection: we used correlations, boxplots, SelectKBest for automatic feature selection, this helped us identify strong predictors for profit.
- Modeling: this included feature scaling in order to standardize our measurement scale for all numeric features, and evaluating different models like Linear Regression, Decision Tree Regressor, K Nearest Neighbours Regressor and Polynomial Regression of different degrees in order to find the model with lowest RMSE score.
- Finally we evaluated the model against the testing set to check for any overfitting and see its prediction power.

Conclusions and Recommendations
-------------------------------
Based on our analysis we provide the following conclusions and recommendations for the future:
- The strongest four key predictors affecting PROFIT_PLAN are INSUR_AMT, GNT_INVEST, CTRCT_AMT_PLAN and R4
- Projects with CNTRY = 10 have a considerably lower mean PROFIT_PLAN than other projects so further analysis is required to discover reasons for this and possibly avoid projects with this attribute value if the reasons cannot be rectified.
- Projects with REGION = 4 have a considerably lower mean PROFIT_PLAN than other projects so further analysis is required to discover reasons for this and possibly avoid projects with this attribute value
- Projects with R7 = 3 and R7 = 5 have the highest mean PROFIT_PLAN so it is recommended to focus more on types of projects with these attribute values and try to replicate the reasons for their higher than average PROFIT_PLAN in other projects.
- Projects with CNTRY = 7 have a considerably higher mean PROFIT_PLAN than other projects so it is recommended to focus more on types of projects with these attribute values and try to replicate the reasons for their higher than average PROFIT_PLAN in other projects.
