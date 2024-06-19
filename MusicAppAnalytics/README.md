# Music App Personalization (Causal Inference)

## Table of Contents
- [Project Overview](#project-overview)
- [Tools and Libraries](#tools-and-libraries)
- [Methodology](#methodology)
- [Results](#results)
- [Recommendations](#recommendations)
- [References](#references)

### Project Overview
This project aims to analyze the causal effect of a new personalization feature on user engagement in a music app. By using causal inference methods, we aim to determine whether exposing users to the new feature increases their interaction with personalized recommendations. The outcome of this analysis will help inform product decisions regarding feature deployment.

### Tools and Libraries
- **Python Version**: 3.9
- **Libraries**:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `causalnex`
  - `dowhy`

### Methodology
1. **Data Preprocessing**: Load and clean the dataset to ensure accuracy in causal analysis.
2. **Exploratory Data Analysis (EDA)**: Perform EDA to understand the data distribution and relationships between variables.
3. **Causal Graph Creation**: Create a causal graph to visualize relationships and identify confounders.
4. **Causal Inference Methods**:
   - **Backdoor Adjustment**: Use backdoor criterion to estimate the causal effect.
   - **Instrumental Variable**: Apply instrumental variable method to estimate causal effect for validation.

### Results
- **Backdoor Adjustment Estimate**: The causal effect estimate using the backdoor adjustment method is \(0.9918\).
- **Instrumental Variable Estimate**: The causal effect estimate using the instrumental variable method is \(0.9778\).

### Recommendations
- Deploy the new personalization feature as it significantly increases user engagement with personalized recommendations.
- Consider additional A/B testing to further validate these findings before a full-scale deployment.
- Monitor user feedback and engagement metrics continuously post-deployment to ensure sustained benefits.

### References
- [DoWhy Documentation](https://www.pywhy.org/dowhy/v0.11.1/)



