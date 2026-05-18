# Student Performance Project

Author: Craig Reynolds

Overview:

This project uses machine learning regression techniques to predict final student grades (G3) based on demographic, social, and academic features.

The goal is to simulate an early intervention system for educators — identifying students at risk of underperforming before final grades are assigned.

To make the problem realistic, early academic grades (G1 and G2) are excluded from model inputs, since they would not be available early in the school year.

Dataset:
Source: UCI Machine Learning Repository
Dataset: Student Performance Dataset (Portuguese secondary school students)
Contains demographic, social, and academic variables

## Tools Used
- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn

## Models Evaluated
- Linear Regression
- Support Vector Regression
- Lasso Regression
- Decision Tree Regression
- Gradient Boosting Regression

Project Workflow

1. Data Exploration & Cleaning
Checked missing values and data types
Investigated feature distributions
Identified noise and sparse categories

2. Feature Engineering
Combined absence variables into a single feature
Merged sparse categorical levels (e.g., education levels 0 & 1)
Encoded categorical variables (One-Hot & Ordinal encoding)
Dropped low-signal features based on EDA

3. Exploratory Data Analysis (EDA)
Correlation heatmaps (Pearson & Spearman)
Grouped mean comparisons for categorical variables
Relationship analysis for key predictors:
Study time
Failures
Parental education
Going out frequency
Alcohol consumption

4. Modeling Approach

Models tested:

Linear Regression
Lasso Regression
Support Vector Regression (SVR)
Decision Tree Regression
Gradient Boosting Regression

Evaluation metric:

Root Mean Squared Error (RMSE) and R²
5. Hyperparameter Tuning
Grid Search applied to Gradient Boosting Regressor
Optimized model complexity vs generalization tradeoff

Final Model Performance
Metric	Score
RMSE	3.86
R²	0.27