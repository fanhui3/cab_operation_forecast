# cab_operation_optimisation
visualization of current ops tempo and forecasting transport demand


# Part 1 - Analytics and story telling of New York Taxi Operations (Task 2)
1. Due to the large file size, dashboard could not be uploaded. Please download the file from the following dropboxlink:
> * https://www.dropbox.com/s/eve4dycnb4yfpmf/dashboard.pbix?dl=0
2. Analysis and recommendations of from the dashboard could be found in the repo in the form of a deck

# Part 2 - TestDome
1. The quiz was attempted within 1 hour and shortly upon receiving the test. However, due to urgent matters arising during the attempt, the attempt was rushed. Nevertheless, the SQL codes compiled with no errors. Please see the 2 amendments that need to be made to attain the required outputs. An email was also sent shortly after the attempt to Jasmine to highlight the corrections needed.

>* Q1. Replace the first line with: *SELECT  department, COUNT(**DISTINCT** employee_id) AS sum_employee FROM employees*. This is to avoid double counting of same employee within the defined period. 
>
>* Q2. Add the following line at the end: ***"WHERE from_date >= "2020-01-01" AND to_date <= 2020-12-31"***. This is to ensure the result is returned from specified date range. 

# part 3 - Forecasting and Demand Prediction (Additional Showcasing)
1. The ipynb enclosed contains the code to predict taxi demand in the **specifed zone for any given hour** using:
>* Hypertuned RandomForest Predictor (81.5% R2 Score)
>* XGBoost Predictor (85.0% R2 Score)
>* ARIMA Time Series Forecasting 

2. To set up, place the following csv in the same location of the ipynb:
>* tripdata.csv (cannot be uploaded on this repo due to file size issue)
>* taxi_zone_lookup.csv

3. To initiate. Ensure the following:
>* Install the required packages listed in the first cell of the notebook
>* Define the zones you are predicting/forecast in the **"target_zone"** variable in cell 2

4. Points of improvments. 
* The data contains only 7 days of taxi operations. Therefore, there are only 1 of each day of week (e.g. monday, tuesday, etc). Therefore, the current iterations of the machine learning models classifies the date input as either a weekday or a weekend. Data from a wider range of date can be included to train the model to enable training of model using each day of week. This allows the model to capture the change in demand over the week and to increase prediction accuracy.   
