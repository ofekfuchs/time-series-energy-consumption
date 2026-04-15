# Time Series Analysis Project - U.S. Energy Consumption

Comprehensive time-series analysis and forecasting project focused on **monthly U.S. total primary energy consumption**.

This repository includes full exploratory analysis, multiple forecasting approaches, exogenous-variable modeling, and change-point detection in one main notebook.

## Authors

- Ofek Fuchs
- Ilana Shmain

## Repository Contents

- `Time_Series_Analysis_Project.ipynb` - Main notebook (full analysis and results)
- `merged_data.csv` - Processed/merged dataset used in the project

## Project Scope

The notebook is organized into four main parts:

1. **Data selection, preprocessing, and visualization**
   - Data filtering and date cleaning
   - Trend/seasonality analysis
   - Stationarity checks (ADF)
   - Additional exploratory visualizations

2. **Model fitting and forecasting**
   - SARIMA / SARIMAX variants
   - Holt-Winters Exponential Smoothing
   - Prophet
   - Regression with Fourier terms
   - LSTM deep learning model
   - Model comparison using `MSE`, `RMSE`, and `MAE`

3. **Exogenous variable integration**
   - Temperature as an exogenous driver
   - Engineered weather features (HDD/CDD and related indicators)
   - Comparative forecast performance with and without exogenous inputs

4. **Change-point detection**
   - Structural-break identification
   - Forecasting with change-point-informed features

## Key Features

- End-to-end workflow: from raw data preparation to model evaluation
- Multiple statistical and ML/DL forecasting approaches in a single pipeline
- Rich visual outputs for trends, seasonality, and forecast comparison
- Reproducible notebook with clear sectioning and outputs

## Data Source

Energy consumption data was collected from the U.S. Energy Information Administration (EIA) endpoint used directly in the notebook:

- [EIA Total Energy Data Browser](https://www.eia.gov/totalenergy/data/browser/)

## How To Run

1. Clone/download this repository.
2. Open the notebook:
   - `Time_Series_Analysis_Project.ipynb`
3. Run all cells in order.

Recommended environment:
- Python 3.9+
- Jupyter Notebook / JupyterLab
- Core libraries used in the notebook include:
  - `pandas`, `numpy`, `matplotlib`, `seaborn`
  - `statsmodels`
  - `prophet`
  - `scikit-learn`
  - `torch` (for LSTM section)

## Notes

- The notebook already includes saved cell outputs, so plots and results are visible directly on GitHub.
