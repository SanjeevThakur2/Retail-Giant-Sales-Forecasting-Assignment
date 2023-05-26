# <font color=black> <div align="center"><u style="border-bottom: 2px solid" >Retail Giant Sales & Quantity Forecasting Assignment</u>

## Problem Statement

Global Mart, an online supergiant store with worldwide operations, is looking to forecast sales and quantity for the next 6 months. As a sales manager, your task is to estimate the demand and plan inventory and business processes accordingly. The dataset provided includes attributes such as order date, segment, market, sales, quantity, and profit.

To determine the most consistently profitable market segment, the coefficient of variation (CoV) will be used. The CoV, which is the ratio of the standard deviation to the mean, allows for a comparison of variance between market segments.

The assignment can be divided into two main problem statements:

## Problem Statement I - Data Preparation

In this step, the focus is on data preparation and identifying the most profitable market segment:

1. Identify the 21 unique market segments.
2. Calculate the CoV for each market segment.
3. Determine the most profitable market segment based on the CoV values.

Transform the order date into the required month-year format and create a time series dataset by concatenating the market and segment columns. Split the dataset into training and test sets, with the test data covering a 6-month period.

## Problem Statement II - Model Building & Evaluation

Once the most profitable market segment is identified, the next step is to forecast sales and quantity for that segment using appropriate techniques:

1. Analyze sales variation for the chosen market segment, considering trends and seasonality.
2. Apply smoothing techniques:
   - Simple exponential smoothing
   - Holt's exponential smoothing
   - Holt-Winters' exponential smoothing (additive and multiplicative techniques)

   Compare the forecasted values with the actual values and calculate the Mean Absolute Percentage Error (MAPE) for each technique.

3. Apply the ARIMA set of techniques (p=1, q=1, d=1):
   - AR model
   - MA model
   - ARMA model
   - ARIMA model
   - ARIMAX model (consider exogenous variables)
   - SARIMA model
   - SARIMAX model (consider exogenous variables)

   Compare the forecasted values with the actual values and calculate the MAPE for each technique.

Repeat the above steps for quantity forecasting on the same market segment used for sales forecasting.

## Insights

Based on the analysis, the Seasonal AutoRegressive Integrated Moving Average (SARIMA) model provided the best results with a Root Mean Square Error (RMSE) of 9617.98 and Mean Absolute Percentage Error (MAPE) of 12.88. These values indicate the accuracy of the SARIMA model in predicting sales for the next 6 months.

Please refer to the Jupyter notebook or presentation for detailed documentation, including CoV values, forecasting methods, trends, and insights.
