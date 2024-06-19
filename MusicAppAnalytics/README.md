# Music App Causal Inference Personalization

## Table of Contents
- [Project Overview](#project-overview)
- [Tools and Libraries](#tools-and-libraries)
- [Methodology](#methodology)
- [Results](#results)
- [Recommendations](#recommendations)
- [References](#references)

### Project Overview
This project aims to analyze the causal effect of a new personalization feature on user engagement in a music app. By using causal inference methods, the goal is to determine whether receiving personalized recommendations increases the hours of content consumed.

### Tools and Libraries
- **Python Version:** 3.9
- **Libraries:**
  - pandas
  - numpy
  - dowhy
  - statsmodels

### Methodology
1. **Simulating Dataset:**
   - Simulate a dataset including relevant variables: PersonalizedRecommendation, HoursOfContentConsumed, UserEngagementLevel, PreferredContentType, NewFeatureExposure.
   
   ![Variable Table](MusicAppAnalytics/Pasted Graphic 4.png)
   
2. **Initializing a Causal Model:**
   - Create a causal graph using the DoWhy library to specify the treatment, outcome, and graph.

3. **Benchmarking with Naive Regression:**
   - Perform a naive regression to get a preliminary understanding of the relationships between variables.

4. **Determining Causal Estimate:**
   - Use DoWhy to estimate the causal effect, controlling for confounders using the backdoor criterion.

5. **Comparing Bias Reduction:**
   - Compare the naive regression estimate and the causal estimate to assess bias reduction.

6. **Stress Testing / Sensitivity Analysis:**
   - Conduct sensitivity analysis to check the robustness of the causal effect estimate to unobserved confounders.
   
   ![Effect of Unobserved Common Cause](MusicAppAnalytics/Effect of Unobserved Common Cause.png)

7. **Alternative Causal Strategies:**
   - Explore the use of instrumental variables to estimate the causal effect as a robustness check.

### Results
- **Naive Regression Estimate:**
  - Slope coefficient: 1.1475
  - Overestimation by approximately 15% due to confounders.
  
- **Causal Effect Estimate (DoWhy - Backdoor Criterion):**
  - Estimated causal effect: 0.9996
  
- **Bias Reduction:**
  - Percentage reduction in bias: 99.71%
  
- **Sensitivity Analysis:**
  - New estimated effect range: -0.271 to 0.881
  - Indicates potential impact of unobserved confounders.
  
- **Alternative Causal Effect Estimate (Instrumental Variable):**
  - Estimated causal effect: 0.9778
  - Slightly less accurate but more robust due to weaker assumptions.

### Recommendations
- Implement personalized recommendations cautiously, ensuring confounders are controlled.
- Consider sensitivity analyses regularly to check for potential biases.
- Use instrumental variables as an alternative causal strategy for robust results.

### References
- [DoWhy Docs](https://www.pywhy.org/dowhy/v0.11.1/)
- [Datacamp Tutorial](https://www.datacamp.com/tutorial/intro-to-causal-ai-using-the-dowhy-library-in-python)


