# Client-churn-rate-prediction-using-ML-model
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

Churn quantifies the number of users who have uninstalled the Waze app or stopped using the app in a given time period. The focus here is on monthly user churn. A high churn rate can indicate dissatifaction of Waze's users and will affect adversely the growth rate of the business. Therefore, using machine learning model to predict user churn can help the management and other stakeholders to take specific and concrete actions to prevent churn and thus to increase user retention rates and stimulate business growth.


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


## **Modeling and evaluation**
## **Conclusion**

hahaha
