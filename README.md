# cab_operation_optimisation
visualization of current ops tempo and forecasting transport demand


# Part 1 - Analytics and story telling of New York Taxi Operations (Task 2)
1. Due to the large file size, dashboard could not be uploaded. Please download the file from the following dropboxlink:
> * https://www.dropbox.com/s/eve4dycnb4yfpmf/dashboard.pbix?dl=0
2. Analysis and recommendations of the file could be found in the repo in the form of a deck

# Part 2 - TestDome
1. The quiz was attempted within 1 hour shortly upon receiving the test. However, due to urgent matters arising during the attempt, the attempt was rush. Nevertheless, the SQL code compiled with no errors. Please see the 2 amendments that needs to be made to attain the required output. An email was sent shortly after Jasmine to highlight the correction needed.

>* Q1. replace the first line with: SELECT  department, COUNT(**DISTINCT** employee_id) AS sum_employee FROM employees. This is to avoid double counting of same employee within the defined period. 
>
>* Q2. add the following line at the end. SELECT  department, **"WHERE from_date >= "2020-01-01" AND to_date <= 2020-12-31"** This is to ensure the result is returned from specified date range. 

# part 3 - Forecasting and Demand Prediction (Additional Showcasing)
1. The ipynb enclosed contains the old to predict taxi demand in the **specifed zone** using:
>* Hypertuned RandomForest Predictor
>* XGBoost Predictor
>* ARIMA Time Series Forecasting 
