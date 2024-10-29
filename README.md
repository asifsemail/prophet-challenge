### Author

	•	Name: Asif Khan
	•	Date: October 2024
	•	Module: Module 8 Challenge - Making Predictions with Data

# MercadoLibre Search Traffic Analysis and Forecasting

This project focuses on analyzing and forecasting search traffic data for MercadoLibre using historical Google search data. The analysis aims to uncover patterns, seasonality, and potential correlations between search traffic and stock price movements. A time series forecasting model is also developed to predict future search trends, providing insights into popular times and days for the platform.

## Project Overview

The project is divided into four main steps:

	1.	Finding Unusual Patterns in Hourly Google Search Traffic
	2.	Mining the Search Traffic Data for Seasonality
	3.	Relating the Search Traffic to Stock Price Patterns
	4.	Creating a Time Series Model with Prophet

Each step includes specific tasks, calculations, and visualizations to answer key questions about the search traffic patterns and their relationship with financial data.

## Instructions and Steps

### Step 1: Find Unusual Patterns in Hourly Google Search Traffic

In this step, we examine Google search traffic data to identify any unusual patterns that may align with MercadoLibre’s quarterly financial results.

	•	1.1: Load and slice the data to May 2020. Visualize to identify unusual patterns.
	•	1.2: Calculate the total search traffic for May 2020 and compare it to the median monthly traffic.
	•	1.3: Determine if there was an increase in search traffic during the month of financial release.

### Step 2: Mine the Search Traffic Data for Seasonality

Analyze the search traffic data to determine daily, weekly, and yearly patterns, which can provide insights into the best times for targeted marketing.

	•	2.1: Plot average traffic by hour of the day.
	•	2.2: Plot average traffic by day of the week.
	•	2.3: Plot average traffic by week of the year.
	•	2.4: Identify any clear time-based trends in search traffic.

### Step 3: Relate the Search Traffic to Stock Price Patterns

Investigate the relationship between search traffic and stock prices to see if there’s a correlation or lagged effect.

	•	3.1: Load and concatenate stock price data with search traffic data.
	•	3.2: Slice data to the first half of 2020 and visualize trends to find a common pattern.
	•	3.3: Create a “Lagged Search Trends” column to offset search traffic by one hour.
	•	3.4: Add two additional columns:
	•	Stock Volatility: A 4-hour exponentially weighted rolling average of stock price volatility.
	•	Hourly Stock Return: Hourly percent change in the stock price.
	•	3.5: Analyze the correlation between lagged search traffic, stock volatility, and hourly stock returns.

### Step 4: Create a Time Series Model with Prophet

Build a forecasting model using Prophet to predict future trends in search traffic and identify specific seasonal patterns.

	•	4.1: Prepare the search data for Prophet by renaming and formatting the columns.
	•	4.2: Fit the Prophet model and generate a forecast.
	•	4.3: Plot the forecast and answer the question: What is the near-term forecast for MercadoLibre’s popularity?
	•	4.4: Use the plot_components function to analyze the following patterns:
	•	Time of Day: Identify the peak hours for search traffic.
	•	Day of the Week: Determine the days with the highest search interest.
	•	Lowest Point in the Calendar Year: Find when search traffic is at its lowest.

## Files

	•	google_hourly_search_trends.csv: Contains Google hourly search data for MercadoLibre.
	•	stock_price_data.csv: Provides historical stock price data for MercadoLibre.
	•	Prophet_Forecast.ipynb: Jupyter Notebook with full code for data analysis and forecasting.

## Requirements

	•	Python Libraries: pandas, Prophet, matplotlib, numpy
	•	Environment: Jupyter Notebook or any Python environment with the necessary libraries installed

## Usage

	1.	Clone this repository and navigate to the project directory.
	2.	Load the Jupyter Notebook Prophet_Forecast.ipynb.
	3.	Run each cell step-by-step to reproduce the analysis, visualizations, and forecasts.
	4.	Review each section to understand the data trends and forecasted results.

## Key Insights and Questions Answered

	1.	Was there an increase in search traffic during financial result releases?
	2.	What time of day and day of the week exhibit the highest search popularity?
	3.	Is there a correlation between search traffic and stock volatility or returns?
	4.	How does the near-term forecast predict future search trends for MercadoLibre?

