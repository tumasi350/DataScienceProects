# Forecasting E-commerce Demand Using Pyspark

## Project Overview

Developed a forecasting model to predict e-commerce demand using retail data. The project utilized PySpark for data processing and model building, achieving a Mean Absolute Error (MAE) of 20.79 using Linear Regression. The process included data aggregation, train-test split, and testing multiple regression models to identify the best-performing one.

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools and Libraries](#tools-and-libraries)
- [Data Aggregation](#data-aggregation)
- [Train Test Split](#train-test-split)
- [Model Building](#model-building)
- [Results/Findings](#resultsfindings)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)

## Data Sources

- `online_retail.csv`: Contains transactional data for online retail.

## Tools and Libraries

- **Python Version:** 3.9
- **Libraries:** 
  - `pyspark`
  - `pandas`

## Data Aggregation

In the initial data preparation phase, the following tasks were performed:
1. Data loading and inspection.
2. Conversion of `InvoiceDate` to a timestamp.
3. Extraction of additional date features (Year, Month, Week, Day, DayOfWeek).
4. Aggregation of data into daily intervals.

## Train Test Split

The data was split into training and test sets based on the date `2011-09-25`:
- Training set: Data before `2011-09-25`.
- Test set: Data on and after `2011-09-25`.

## Model Building

Included models:
1. **Random Forest Regressor**
2. **Linear Regression**
3. **Decision Tree Regressor**
4. **Gradient-Boosted Trees (GBT) Regressor**

Models were evaluated using the Mean Absolute Error (MAE) metric to determine their performance.

## Results/Findings

The Linear Regression model performed best among the tested models, achieving an MAE of 20.79. The Random Forest Regressor and Decision Tree Regressor showed higher MAE values, indicating lower accuracy.

## Recommendations

Based on the analysis, the following actions are recommended:
- **Feature Engineering**: Explore additional features, such as promotional activities, economic indicators, seasonality adjustments, or customer demographics to enhance model accuracy.
- **Model Tuning**: Fine-tune the parameters of the Linear Regression model or explore other algorithms that might better capture non-linear relationships.
- **Data Augmentation**: Increase the dataset size or incorporate external datasets to improve model performance.

## Limitations

The model showed an overestimation of demand for certain periods, indicating that there may be underlying patterns or factors not captured effectively by the current features and model setup.

## References

1. [UCI Machine Learning Repository - Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)
