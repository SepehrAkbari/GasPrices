# Imputing Daily Gas Prices

## Overview

This project investigates efficient data collection methods for time-series data, specifically focusing on inferring daily gas price values from weekly records. By comparing Linear Approximation and a quadratic Taylor Series, the project aims to achieve accurate daily imputations with minimized data demands, making it a valuable approach for data efficiency in forecasting and reducing storage and processing needs.

## Project Structure

- **main.ipynb**: Contains the full code and analysis for the project, including data loading, imputation methods, comparisons, and visualizations of results.
- **gas_price_data.txt**: Source data file containing weekly gas prices (ensure this is placed in the same directory for seamless execution).

## Methods

### 1. Linear Approximation
The Linear Approximation approach leverages a straightforward linear regression model to estimate daily values between weekly data points. This method prioritizes simplicity and computational efficiency.

### 2. Quadratic Taylor Series
The Taylor Series method expands upon the linear approach by incorporating a second-order term, allowing for curvature in the estimated data. This approach is particularly useful in markets with high variability.

## Results

The analysis demonstrates:
- **Accuracy**: Taylor Series shows higher accuracy in fluctuating markets, while Linear Approximation provides a good balance of speed and simplicity.
- **Application in Extrapolation**: Both methods have been tested for interpolation and extrapolation, with Taylor Series performing well in both contexts.

## Getting Started

### Prerequisites
- Python 3.x
- Required libraries: `pandas`, `numpy`, `matplotlib`, `sklearn`

Install any missing packages using:
```bash
pip install pandas numpy matplotlib scikit-learn
```
