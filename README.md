# Electricity Demand Forecasting using Time Series Analysis

## Project Overview

This project focuses on forecasting monthly electricity consumption demand for the next 1–2 years using historical electricity consumption data from January 1973 to December 2019.

The objective is to help electricity distribution companies accurately estimate future demand for better production planning, vendor management, and resource allocation.

The project compares multiple time series forecasting models including:

- Time Series Decomposition
- ETS (Exponential Smoothing)
- ARIMA
- SARIMA

The models are evaluated using standard forecasting accuracy metrics such as RMSE, MAPE, and RMSPE.

---

## Business Problem

Electricity distribution companies require accurate demand forecasting to:

- Avoid underproduction and overproduction
- Optimize electricity procurement
- Improve vendor and supply chain management
- Plan future infrastructure and operational requirements

This project aims to build a robust forecasting solution for monthly electricity demand prediction.

---

## Dataset Information

### Features

| Column | Description |
|---|---|
| Date | Month & Year |
| Electricity Consumption | Electricity consumption in Trillion Watts |

### Data Duration

- Start Date: January 1973
- End Date: December 2019
- Frequency: Monthly

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- Scikit-learn

---

## Project Workflow

1. Data Loading and Preprocessing
2. Exploratory Data Analysis (EDA)
3. Time Series Visualization
4. Seasonal Decomposition
5. Train-Test Split
6. Model Building
    - ETS Model
    - ARIMA Model
    - SARIMA Model
7. Model Evaluation
8. Forecast Generation
9. Business Insights and Conclusion

---

## Forecasting Models Used

### 1. ETS (Exponential Smoothing)

Used to capture trend and seasonality in the data.

### 2. ARIMA

Captures autoregressive and moving average components after differencing stationary data.

### 3. SARIMA

Handles both non-seasonal and seasonal patterns in monthly electricity demand data.

---

## Evaluation Metrics

The following metrics were used to compare model performance:

- RMSE (Root Mean Square Error)
- MAPE (Mean Absolute Percentage Error)
- RMSPE (Root Mean Square Percentage Error)

---

## Results

After comparing all forecasting models, the best-performing model was selected based on:

- Lowest forecasting error
- Ability to capture seasonality
- Stability of predictions

The selected model was then used to forecast electricity demand for the next 24 months.

---

## Project Structure

```text
electricity-demand-forecasting/
│
├── data/
│   └── electricity_consumption.csv
│
├── notebooks/
│   └── Electricity_Demand_Forecasting.ipynb
│
├── outputs/
│   ├── forecast_plot.png
│   └── model_metrics.csv
│
├── README.md
├── requirements.txt
└── .gitignore
