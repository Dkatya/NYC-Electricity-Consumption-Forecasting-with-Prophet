# NYC-Electricity-Consumption-Forecasting-with-Prophet

This repository contains a time series forecasting project that predicts New York City's electricity consumption using Facebook's Prophet model. The project analyzes monthly and yearly electricity consumption data to create accurate forecasts at different time scales.

## Project Overview

This project implements a time-agnostic forecasting system that automatically detects the time unit (month, year) from input data and adjusts prediction horizons accordingly. The Prophet model is tuned with various parameters to optimize forecasting accuracy across different time scales.

### Key Features

- **Time-Agnostic Forecasting**: Automatically detects and adapts to monthly or yearly time series data
- **Multi-Horizon Predictions**: 
  - For monthly data: 1, 6, and 9 months into the future
  - For yearly data: 1, 3, and 5 years into the future
- **Comprehensive Model Tuning**:
  - Testing different growth models (logistic, linear, flat)
  - Custom seasonality configurations
  - Optimized trend changepoints

### Performance Metrics

Each model is evaluated using:
- Mean Absolute Error (MAE)
- Mean Absolute Percentage Error (MAPE)
- R-squared (R²)

## Dataset

The project utilizes historical New York City electricity consumption data at two different aggregation levels:
- Monthly mean consumption (derived from daily data)
- Yearly mean consumption (derived from daily data)

## Implementation

The entire project is implemented in Python using a Jupyter Notebook, with the following key components:
- Data preprocessing and aggregation
- Time unit detection algorithm
- Prophet model implementation with parameter tuning
- Visualization of historical and forecasted data
- Model evaluation and comparison

## Dependencies

- Python 3.x
- fbprophet
- pandas
- numpy
- matplotlib
- sklearn

## Getting Started

1. Clone this repository
2. Install the required dependencies
3. Open the Jupyter Notebook to view the implementation and results

## Results

The notebook includes detailed visualizations comparing historical data with forecasts, alongside comprehensive performance metrics for each model configuration and time scale.
