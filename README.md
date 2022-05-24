# Time-Series---Housing-Market

# 1. Introduction

For this project, I am acting as a consultant for a fictional real-estate investment firm, and I will be forecasting real estate prices of various zip codes using data from Zillow. The goal of the project is to analyze, model, and predict returns in order to recommend the best 5 zipcodes to invest in Gwinnett County, Georgia 

# 2. Dataset

The dataset can be found in this repo which was obtained from Zillow Research Page (https://www.zillow.com/research/data/). It contains nearly 15,000 lines with basic information such as city, state, county, size rank from April 1996 - April 2018. The Gwinnett County portion has 4240 line with 16 zip codes


# 3. Scrub & Explore

In this section, I filtered, check for null values, and melted my dataset. Here is the boxplot to show all 16 zipcodes in Gwinnett County as well as their price ranges.

![alt text](https://raw.githubusercontent.com/helennpham0229/Time-Series---Housing-Market/main/images/gwinnett%20zip%20codes.png)


# 4. Analysis and Modeling

## 4a. Functions

I created 4 functions to help me observe the original dataset and any trends and seasonality component for each zipcode.
- Function 1: stationarity check with Dickey-Fuller test
- Function 2: decompose time series so we can observe trend, seasionality, and residuals
- Function 3: run auto arima and search for the best parameters and then using SARIMAX to fit our models
- Function 4: Gets one-step-ahead forecast for model, Calculates Root of Mean Squared Error, Makes future predictions , Plots results and Provides forecasted value with confidence interval

## 4b. Top 5 Zipcodes
### 30024
![alt text](https://raw.githubusercontent.com/helennpham0229/Time-Series---Housing-Market/main/images/30024%20forecast.png)

### 30043
![alt text](https://raw.githubusercontent.com/helennpham0229/Time-Series---Housing-Market/main/images/30043%20forecast.png)

### 30096
![alt text](https://raw.githubusercontent.com/helennpham0229/Time-Series---Housing-Market/main/images/30096%20forecast.png)

### 30047
![alt text](https://raw.githubusercontent.com/helennpham0229/Time-Series---Housing-Market/main/images/30047%20forecast.png)

### 30045
![alt text](https://raw.githubusercontent.com/helennpham0229/Time-Series---Housing-Market/main/images/30045%20forecast.png)

# 5. Conclusion
![alt text](https://raw.githubusercontent.com/helennpham0229/Time-Series---Housing-Market/main/images/summary%20table.PNG)
