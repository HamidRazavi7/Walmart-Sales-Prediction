# Walmart Sales Prediction: Enhancing Forecasting Accuracy

About the Project

This project develops a predictive model to forecast weekly sales in Walmart stores using historical data from 2010 to 2012. It integrates advanced data preprocessing techniques, model optimization strategies, and time series analysis to achieve robust and accurate predictions.

## Key Features

Data Preprocessing: Outlier detection (IQR method), feature engineering, and missing value imputation.

Machine Learning Models: Gradient Boosting, Random Forests, and Linear Models.

Time Series Analysis: Holt-Winters model for capturing seasonality and trends.

Performance Evaluation: Metrics like RMSE, MAE, and R² scores for model comparison.

## Dataset

The dataset includes:

Weekly sales across 45 Walmart stores.

Features: store ID, holiday flag, temperature, fuel price, CPI, and unemployment rates.

Example:

Feature

Description

Weekly Sales

Target variable (total weekly sales)

Store

Store ID (1-45)

Holiday Flag

Binary indicator for holidays

Temperature

Average weekly temperature (F)

Methodology

Data Preprocessing

Outlier Removal: Using the Interquartile Range (IQR) method.

Feature Selection: PCA retained 7 components capturing 95% variance.

Correlation Analysis: Visualized relationships among features.

Machine Learning Models

Model

Validation R²

Notes

Linear Regression

0.1654

Poor performance, minimal overfitting.

Random Forest

0.6646

Overfit; extensive hyperparameter tuning applied.

Gradient Boosting

0.6757

Best performance; slightly overfit.

Time Series Analysis

Model: Holt-Winters method for trend and seasonality.

Mean Absolute Error: 44,639 (significantly lower than ML models).

## Results

Gradient Boosting achieved the best machine learning results (R² = 0.6671 on the test set).

Time Series analysis highlighted the importance of considering temporal dependencies.

Key Metrics:

Metric

Gradient Boosting

Time Series Model

Mean Absolute Error

218,633

44,639

Root Mean Square Error

329,996.62

-

R²

0.6671

-

Challenges and Future Work

Challenges: Overfitting in ensemble models; limited incorporation of economic variables in time series models.

Future Enhancements:

Explore ARIMA models for advanced time series analysis.

Integrate non-time variables (e.g., CPI, unemployment) into time series models.

## Resources

Dataset on Kaggle

Presentation Video

## Authors

Hamid Razavi

John Fahim

Rajiv Kumar

