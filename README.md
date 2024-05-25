#Time Series Forecasting of NYC Electricity Consumption Using FBProphet

This project focuses on implementing a time series forecasting model in Python to predict electricity consumption in New York City using Facebook's Prophet module. The Prophet model is a robust procedure for forecasting time series data based on an additive model that incorporates non-linear trends with yearly, weekly, and daily seasonality.

##Objective
To accurately forecast New York City's electricity consumption using daily, monthly mean, and yearly mean datasets.

##Dataset
The dataset contains daily electric consumption data for all five boroughs of New York City, spanning from 2010 to February 2023. This dataset can be found here. Monthly and yearly mean data are derived from this daily dataset by averaging the values accordingly.

##Tasks
###Data Preparation:

Load and preprocess the daily electricity consumption data.
Aggregate the daily data to create monthly mean and yearly mean datasets.

###Model Implementation:

Write Python scripts to handle varying time units (daily, monthly, yearly) agnostically.
Train the FBProphet model on each dataset (daily, monthly mean, yearly mean).

###Forecasting:

Predict future electricity consumption values:
Daily data: Forecast for 100/200/365 days into the future.
Monthly mean data: Forecast for 1/6/9 months into the future.
Yearly mean data: Forecast for 1/10/20 years into the future.

###Model Tuning:

Tune the Prophet model parameters:
Forecasting growth options: logistic, linear, flat.
Seasonality: Add manual seasonality using the add_seasonality method, experimenting with different values for period and fourier_order.
Trend Changepoints: Adjust n_changepoints and changepoint_prior_scale.

###Evaluation:

Evaluate the performance of the models using:
Mean Absolute Error (MAE)
Mean Absolute Percentage Error (MAPE)
R-squared (R²)
Visualization and Reporting:

Print the predicted values in a tabular format.
Generate line graphs showing historical data and future predictions.
Document the entire process, findings, and results in a single Jupyter Notebook or Python (.py) file.
