# Client-churn-rate-prediction-using-machine-learning-model
## **Overview**

This project is based on Google Advanced Data Analytics online courses available on Coursera.
The goal of the project is to build machine learning as well as regression model to forecast the client churn rate for Waze, a company providing navigation services to its app users.

Please note while Waze is a real company, the data shared by Coursera/Google here is solely for pedagogical purpose, which is also explicitly stated within Coursera platform.
With this project I will also show the following skillsets that have been obatined:

* EDA (exploratory data analysis)
* Data visulization
* Statitical analysis of the data and regression analysis (logistic regression)
* Machine learning model (decision tree, random forest, XGBoost)

The programming language is Python, including the following liabraries/ packages or modules therein:

* pandas
* numpy
* matplotlib
* seaborn
* sklearn
* scipy
* statsmodels



## **Business understanding**

Churn quantifies the number of users who have uninstalled the Waze app or stopped using the app in a given time period. The focus here is on monthly user churn. A high churn rate can indicate dissatifaction of Waze's users and will affect adversely the growth rate of the business. 

Therefore, using machine learning model to predict user churn can help the management and other stakeholders to take specific and concrete actions to prevent churn and thus to increase user retention rates and stimulate business growth.


## **Data understanding**

The dataset contains 14,999 rows and 13 columns, with each row representing a unique user and each column a specific feature associated with the user. The table below demonstrates the overview of the data.

|Column name |Type |Description
|:-----------------------|:----:|:----------
|label                   |obj   |Binary ("retained" vs. "churned") during the course of the month
|sessions                |int   |The number a user opening the app during the month
|drives                  |int   |An occurrence of driving at least 1 km during the month
|device                  |obj   |The type of device a user starts a session with
|total sessions          |float |A model estimate of the total number of sessions since a user has onboarded
|n_days_after_onboarding |int   |The number of days since a user signed up for the app
|total_navigations_fav1  |int   |Total navigations since onboarding to the user’s favorite place 1
|total_navigations_fav2  |int   |Total navigations since onboarding to the user’s favorite place 2
|driven_km_drives        |float |Total kilometers driven during the month
|duration_minutes_drives |float |Total duration driven in minutes during the month
|activity_days           |int   |Number of days the user opens the app during the month
|driving_days            |int   |Number of days the user drives (at least 1 km) during the month

Apart from the features above, features engineering was also performed to maximize the usage of the data and increase the predictability of the model. For example, 'km_per_driving_day' combined two features ('driven_km_drives' and 'driving_days') to indicate the average number of kilometers driven on each day in the last month for each user. Similarly, 'total_sessions_per_day' used 'total_sessions' and 'n_days_after_onboarding' to represent the average number of sessions on each day since user's onboarding. 

The table below shows all engineered features used in the model.
|Column name |Type |Description
|:-----------------------|:----:|:----------
|km_per_driving_day              |float |Average number of kilometers driven on each driving day in the last last month
|percent_sessions_in_last_month  |float |The precentage of each user's total sessions logged in the last month
|professional_driver             |int   |Users who had 60 or more drives and drove on 15+ days in the last month
|total_sessions_per_day          |float |Average number of sessions per day since onboarding
|km_per_hour                     |float |Average number of kilometers per hour driven in the last month
|km_per_drive                    |float |Average number of kilometers per drive made in the last month for each user
|percent_of_sessions_to_favorite |float |Percentage of total sessions used to navigate to one of the user's favorite places

From the feature importance bar chart (generated from XGBoost model) can be seen that the feature engineering was very effective as 3 out of the top 5 features (6 out of the top 10 features) were not included in the original dataset but engineered during the analysis and model construction.

![alt text](https://github.com/friend-of-data/Client-churn-rate-prediction-using-ML-model/blob/main/Feature_importance.PNG)
## **Modeling and evaluation**
## **Conclusion**

hahaha
