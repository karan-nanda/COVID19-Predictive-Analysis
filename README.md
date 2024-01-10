# COVID19-Predictive-Analysis

# COVID-19 Time Series Analysis and Forecasting

## Introduction

This repository contains Python code for time series analysis and forecasting of COVID-19 data using various models. The dataset used is sourced from the 'COVID-19 Data Repository by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University' also present in the repository. The analysis includes exploratory data analysis (EDA), visualization of confirmed cases, recovered cases, and deaths worldwide, as well as time series forecasting using different models.

## Libraries Used

- `numpy` and `pandas` for data manipulation.
- `matplotlib` and `seaborn` for data visualization.
- `plotly` for interactive and dynamic plots.
- `sklearn` for model selection and evaluation.
- `statsmodels` for time series analysis.
- `pmdarima` for AutoARIMA model selection.
- `pandas_datareader` for fetching COVID-19 data.
- `warnings` to suppress unnecessary warnings.

## Data Loading and Preprocessing

The analysis begins with loading the COVID-19 dataset, checking the data types, and performing basic data preprocessing steps. Unnecessary columns such as 'SNo' and 'Last Update' are dropped, and column names are standardized.

## Exploratory Data Analysis (EDA)

### Confirmed Cases Over Time

The cumulative confirmed cases are plotted over time to visualize the spread of COVID-19 globally. The data is grouped by date, and the cumulative sum is calculated for each day.

### Recovered Cases Over Time

Similar to confirmed cases, the cumulative recovered cases are plotted to observe the recovery trend.

### Deaths Over Time

The cumulative deaths are visualized over time, showing the unfortunate impact of the pandemic globally.

### Active Cases Worldwide

A choropleth map is created to display the active COVID-19 cases worldwide. The color intensity represents the number of confirmed cases in each country.

### Mortality and Recovery Rates

Mortality and recovery rates are calculated and visualized for countries most affected by COVID-19.

### Top Countries with High Mortality and Recovery Rates

The top 15 countries with the highest mortality and recovery rates are visualized in separate bar charts.

## Time Series Forecasting

### Holt's Linear Model

The Holt Linear model is applied to predict the confirmed cases. The model is trained on the historical data, and predictions are compared with the actual test data.

### Holt's Winter Model

A more sophisticated Holt-Winter model is utilized to capture seasonality in the time series data.

### ARIMA, MA, AR, and SARIMA Models

AutoARIMA is employed to automatically select the best parameters for the ARIMA, MA, AR, and SARIMA models. The models are trained, predictions are made, and their performance is evaluated.

### Model Selection - Confirmed Cases

The root mean squared error (RMSE) is used to compare the performance of different models. The SARIMA model is selected as the best model for predicting confirmed cases.

### Model Testing - Deaths

The ARIMA and SARIMA models are tested for predicting deaths. The RMSE is used to compare the models, and the ARIMA model is selected as the best model for death predictions.

## Conclusion

The SARIMA model is identified as the best model for predicting confirmed cases, while the ARIMA model is selected for death predictions. These models provide valuable insights into the trends and help in making informed decisions during the ongoing COVID-19 pandemic. Further improvements and refinements can be made based on evolving data and more advanced modeling techniques.

Feel free to explore the code, run the analyses, and contribute to the improvement of the models!
