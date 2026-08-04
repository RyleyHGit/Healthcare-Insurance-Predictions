# Healthcare Insurance Cost Prediction

A multiple linear regression project focused on identifying the best predictive model for individual healthcare insurance charges. Several model selection techniques were compared, including interaction models, polynomial regression, subset selection, stepwise regression, and cross-validation to determine the model with the strongest predictive performance.

## Project Overview

The objective of this project was to develop and compare multiple regression models for predicting healthcare insurance charges using demographic and health-related variables. Model performance was evaluated using R², Adjusted R², AIC, and cross-validation mean squared error (MSE).

## Dataset

The dataset contains healthcare insurance information with the following predictors:

- Age
- Sex
- BMI (Body Mass Index)
- Number of Children
- Smoking Status
- Region

**Response Variable**

- Insurance Charges

## Key Findings

- Smoking status was the strongest predictor of healthcare costs.
- Age and BMI were the next most influential predictors.
- Strong interaction effects existed between:
  - Age × BMI
  - BMI × Smoking
  - Age × Smoking
  - Age × BMI × Smoking
- Age and BMI also demonstrated nonlinear relationships with insurance charges.

## Best Performing Model

The final selected model included:

- Age
- BMI
- Smoking Status
- Age × BMI
- BMI × Smoking
- Age × Smoking
- Age × BMI × Smoking

### Model Performance

| Metric | Value |
|--------|-------:|
| R² | 0.8368 |
| Adjusted R² | 0.8360 |
| AIC | 22748.55 |

Cross-validation confirmed this model achieved the lowest prediction error among all candidate models.

## Tools

- R
- Multiple Linear Regression
- ANOVA
- Stepwise Regression
- Best Subset Selection
- Cross Validation
