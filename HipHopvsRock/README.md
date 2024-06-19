# Classifying Music Genres Using Echo Nest Data

## Project Overview

Created a machine learning model to classify music tracks as either Hip-Hop or Rock, achieving an accuracy of 82% using logistic regression. The project involved preprocessing and balancing the dataset, applying PCA for dimensionality reduction, and using decision tree and logistic regression models to classify the tracks, with model performance evaluated using cross-validation.

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools and Libraries](#tools-and-libraries)
- [Data Cleaning/Preparation](#data-cleaningpreparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Model Building](#model-building)
- [Results/Findings](#resultsfindings)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)

## Data Sources

- `fma-rock-vs-hiphop.csv`: Contains detailed information about music tracks.
- `echonest-metrics.json`: Contains Echo Nest audio features for the tracks.

## Tools and Libraries

- **Python Version:** 3.9
- **Libraries:** 
  - `pandas`
  - `numpy`
  - `sklearn`
  - `matplotlib`

## Data Cleaning/Preparation

In the initial data preparation phase, the following tasks were performed:
1. Data loading and inspection.
2. Handling missing values.
3. Data cleaning and formatting.

## Exploratory Data Analysis

EDA involved exploring the music data to answer key questions, such as:
- What are the distributions of different features?
- Are there any strong correlations between the features?

## Model Building

Included models:
1. **Decision Tree Classifier**
2. **Logistic Regression**

Both models were evaluated using cross-validation to determine their performance.

## Results/Findings

The logistic regression model performed better than the decision tree model, achieving an accuracy of 82%, compared to the decision tree's accuracy of 80%.

## Recommendations

Based on the analysis, the following actions are recommended:
- **Data Augmentation**: Increase the size of the Hip-Hop track dataset to improve model balance and performance.
- **Feature Engineering**: Explore additional features or different combinations of existing features to enhance model accuracy.
- **Model Tuning**: Further tune the hyperparameters of the logistic regression model to potentially improve accuracy beyond 82%.
- **Alternative Models**: Experiment with other classification models like Random Forest or SVM to see if they offer better performance.

## Limitations

The model showed bias toward the Rock classification due to an imbalanced dataset. Balancing the dataset improved model performance.

## References

1. [Million Song Dataset](http://millionsongdataset.com/)
