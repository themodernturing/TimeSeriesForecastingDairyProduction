# Time Series Analysis of California Dairy Data

This repository contains a Jupyter Notebook (`TimeSeries.ipynb`) that explores and models a time series dataset of California dairy production. The analysis encompasses data loading, exploratory data analysis, time series decomposition, and forecasting using ARIMA models.

## Project Overview

This project aims to:

* **Explore the characteristics** of the California dairy production time series.
* **Decompose** the time series into trend, seasonal, and residual components.
* **Apply time series models** (ARIMA) to the residual component.
* **Forecast** monthly milk production for a 12-month period.

## Files

* `TimeSeries.ipynb`: The Jupyter Notebook containing the time series analysis and forecasting.
* `cadairydata.csv`: (This file is assumed to be part of the project or required to run the notebook, though the notebook shows it is downloaded from a workspace) The California dairy production dataset.

## Data Description

The `cadairydata.csv` dataset contains monthly data on California dairy production, including information on milk production, ice cream production, and related factors. The time series spans several years, exhibiting trends and seasonal patterns.

## Methodology

The analysis within the notebook follows these key steps:

1.  **Data Loading and Preprocessing:**
    * Loading the dataset.
    * Creating a POSIXct time series object from year and month information.
    * Converting the Month column to an ordered factor.
    * Cleaning and preparing the data for analysis.

2.  **Exploratory Data Analysis (EDA):**
    * Visualizing time series plots of milk and ice cream production.
    * Examining statistical properties of the time series, including autocorrelation (ACF and PACF) and data distribution (histograms).

3.  **Time Series Decomposition:**
    * Decomposing the time series into trend, seasonal, and remainder components using:
        * Simple moving average decomposition.
        * STL (Seasonal-Trend decomposition using Loess) decomposition.

4.  **ARIMA Modeling:**
    * Modeling the remainder component of the time series using Autoregressive Integrated Moving Average (ARIMA) models.
    * Fitting ARIMA models to the time series data.

5.  **Forecasting:**
    * Using the `forecast` package in R to automatically determine and apply an ARIMA model.
    * Forecasting milk and ice cream production for a 12-month period.
    * Visualizing the forecast with confidence intervals.

## Libraries and Tools

The analysis is performed using the following R libraries:

* `AzureML`: (If applicable) For accessing the dataset within Azure Machine Learning.
* `ggplot2`: For data visualization.
* `gridExtra`: For arranging multiple plots.
* `forecast`: For ARIMA modeling and forecasting.

## Usage

1.  Clone this repository to your local machine.
2.  Open the `TimeSeries.ipynb` notebook in a suitable environment (e.g., Jupyter Notebook, RStudio).
3.  Ensure you have the required R libraries installed.
4.  Run the cells in the notebook to reproduce the analysis and forecasting.

## Key Findings

The notebook explores the decomposition of time series data and applies ARIMA modeling to forecast future production. The analysis provides insights into:

* Trend and seasonality in dairy production.
* The effectiveness of different decomposition methods.
* The application of ARIMA models for time series forecasting.

## Contributing

Contributions to this project are welcome. Feel free to fork the repository, implement improvements, and submit pull requests.

## License

