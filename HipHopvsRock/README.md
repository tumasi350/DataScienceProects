# Classifying Music Genres Using Echo Nest Data

## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools and Libraries](#tools-and-libraries)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Principal Component Analysis (PCA)](#principal-component-analysis-pca)
- [Model Building](#model-building)
- [Model Evaluation](#model-evaluation)
- [Balancing the Dataset](#balancing-the-dataset)
- [Cross-Validation](#cross-validation)
- [Conclusion](#conclusion)

## Project Overview
Created a machine learning model to classify music tracks as either Hip-Hop or Rock, achieving an accuracy of 82% using logistic regression. The project involved preprocessing and balancing the dataset, applying PCA for dimensionality reduction, and using decision tree and logistic regression models to classify the tracks, with model performance evaluated using cross-validation.

## Data Sources
- **Echo Nest Data**: Contains various audio features for the tracks.
- **FMA Dataset**: Metadata for the tracks used for genre classification.

## Tools and Libraries
- **Python Version:** 3.9  
- **Libraries:** pandas, numpy, sklearn.model_selection (train_test_split, KFold, cross_val_score), sklearn.preprocessing (StandardScaler), matplotlib.pyplot, sklearn.decomposition (PCA), sklearn.linear_model (LogisticRegression), sklearn.metrics (classification_report), sklearn.tree (DecisionTreeClassifier), sklearn.pipeline (Pipeline)  

## Data Cleaning and Preparation
- **Data Merging**: Merged Echo Nest metrics with track metadata using track IDs.
- **Missing Values**: Handled missing values appropriately.
- **Feature Engineering**: Parsed and created new features from the existing data.

## Exploratory Data Analysis (EDA)
- **Correlation Matrix**: Identified redundancies in data using a correlation matrix to maintain model efficiency and clarity.
- **Feature Selection**: Selected relevant features for modeling.

## Principal Component Analysis (PCA)
- **Variance Explained**: Used scree plots and cumulative explained variance plots to determine the optimal number of components.
- **Dimensionality Reduction**: Reduced the dataset to 6 principal components explaining 85% of the variance.

## Model Building
- **Decision Tree**: Built a decision tree classifier to categorize tracks.
- **Logistic Regression**: Built a logistic regression model for comparison.

## Model Evaluation
- **Metrics**: Evaluated models using precision, recall, and f1-score.
- **Results**: Logistic regression performed better than the decision tree, with a higher overall accuracy.

## Balancing the Dataset
- **Balancing**: Balanced the dataset to address model bias towards the "Rock" classification by adjusting class weights.
- **Impact**: Improved model fairness and classification accuracy.

## Cross-Validation
- **K-Fold Cross-Validation**: Implemented cross-validation to rigorously evaluate model performance.
- **Comparison**: Logistic regression consistently outperformed the decision tree.

## Conclusion
The logistic regression model achieved higher accuracy and better overall performance compared to the decision tree model for classifying music genres. This project demonstrates the importance of data preprocessing, dimensionality reduction, and model evaluation techniques in building effective machine learning models.

