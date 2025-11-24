---
slug: github-sales-forecasting
title: Sales Forecasting Project Using Naive Models and Data Resampling
repo: justin-napolitano/sales-forecasting
githubUrl: https://github.com/justin-napolitano/sales-forecasting
generatedAt: '2025-11-23T09:34:12.161596Z'
source: github-auto
summary: >-
  Analysis of historical sales data with naive forecasting methods, data preprocessing, evaluation
  metrics, and future modeling plans.
tags:
  - sales-forecasting
  - time-series
  - pandas
  - model-evaluation
seoPrimaryKeyword: sales forecasting
seoSecondaryKeywords:
  - time series forecasting
  - naive models
  - data preprocessing
  - model evaluation
seoOptimized: true
---

# Sales Forecasting Project

## Motivation

Accurate sales forecasting is critical for inventory management, resource allocation, and strategic planning. This project aims to analyze historical sales data to evaluate forecasting methods and establish a baseline for future predictive modeling.

## Problem Statement

The core problem addressed is the prediction of daily sales volumes based on past sales data. The dataset contains timestamped sales counts aggregated hourly and daily. The challenge is to develop models that can accurately forecast sales to inform business decisions.

## Project Overview

The project consists of data ingestion, preprocessing, exploratory analysis, model implementation, and evaluation. The primary data source is a CSV file logging sales counts by date, hour, day of week, and week number.

### Data Handling

Data is loaded using pandas and resampled to daily frequency by summing hourly sales. This aggregation simplifies modeling and aligns with typical business reporting periods.

### Modeling Approach

Initial models implemented are naive forecasting methods, which predict sales for a given day as equal to the previous day's sales. This approach serves as a baseline to compare more advanced models against.

### Evaluation Metrics

Model performance is assessed using Root Mean Squared Error (RMSE) and Mean Absolute Percentage Error (MAPE). These metrics quantify prediction accuracy and relative error, respectively.

### Implementation Details

- The script `salesforecasting.py` contains functions to compute MAPE and to prepare the data.
- Data is split into historic (January and February) and test (March) periods to evaluate model performance on unseen data.
- Visualization uses matplotlib to plot sales trends and model predictions for comparison.

### Current Limitations

- Forecasting is limited to naive methods; no advanced predictive models are yet implemented.
- Prediction functionality for future dates is not yet available; the focus is on validating models against historical data.
- Visualization of forecasts is basic and requires enhancement for clarity.

## Practical Notes

- Data preprocessing includes converting date strings to datetime objects and resampling to daily sums.
- Error dictionaries are used to store and compare model performance metrics.
- The code assumes the data file path is set correctly; this may require adjustment for different environments.

## Next Steps

- Implement predictive models capable of forecasting future sales beyond the test period.
- Explore time series models such as ARIMA or machine learning models for improved accuracy.
- Refine evaluation by incorporating cross-validation and additional error metrics.
- Enhance plotting to better visualize forecast uncertainty and model comparisons.
- Automate data ingestion and model evaluation pipelines for scalability.

This documentation serves as a technical reference for returning developers to understand the project's structure, current state, and planned directions without extraneous commentary or motivational language.
