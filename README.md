# sales-forecasting

This repository contains code and data for analyzing and modeling sales data with the goal of forecasting future sales. The project primarily uses Jupyter Notebooks and Python scripts to explore historical sales data, evaluate forecasting models, and visualize results.

## Features

- Data aggregation and preprocessing of sales logs
- Implementation of baseline forecasting models such as naive forecasting
- Evaluation metrics including RMSE and MAPE for model performance
- Visualization of sales trends and model predictions

## Tech Stack

- Python 3
- Jupyter Notebook
- pandas for data manipulation
- numpy for numerical operations
- matplotlib for plotting
- statsmodels for statistical modeling
- scikit-learn for error metrics

## Getting Started

### Prerequisites

Ensure you have Python 3 installed along with the required packages. It is recommended to use a virtual environment.

### Installation

```bash
pip install pandas numpy matplotlib statsmodels scikit-learn
```

### Running the Project

1. Load the dataset `PotLog.csv` into the working directory.
2. Open and run the Jupyter Notebook `SalesForcasting.ipynb` to explore the data and models.
3. Alternatively, run the Python script `salesforecasting.py` to execute the forecasting code.

## Project Structure

- `PotLog.csv` - Raw sales data with timestamps and sales counts.
- `SalesForcasting.ipynb` - Jupyter Notebook for interactive exploration and modeling.
- `salesforecasting.py` - Python script containing forecasting model implementations and evaluation.
- `README.md` - Project documentation.

## Future Work / Roadmap

- Extend forecasting models to generate future sales predictions beyond validation.
- Improve visualization to better represent forecast uncertainty.
- Add more sophisticated models such as ARIMA, Prophet, or machine learning approaches.
- Implement automated model selection based on performance metrics.
- Include weekly or multi-week forecasting capability.
- Enhance documentation and add usage examples.
