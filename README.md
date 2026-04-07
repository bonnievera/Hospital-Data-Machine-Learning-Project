# Hospital-Data-Machine-Learning
Goal: To predict patient readmission using linear and non-parametric machine learning models.

# Project Overview

Hospital readmissions are a major challenge in healthcare, leading to increased costs and patient risk.

The goal of this project is to:

- Predict whether a patient will be readmitted (yes/no)
- Identify key factors influencing readmission
- Compare multiple machine learning models

# Key Features:
-Patient demographics (age)
-Hospital usage (time in hospital, inpatient visits)
-Medical activity (lab procedures, medications)
-Diagnosis categories
-Diabetes-related tests (A1C, glucose)

# Machine Learning Workflow

This project follows a structured ML pipeline:

Data Loading
-Exploratory Data Analysis (EDA)
-Data Preprocessing
-Feature Encoding
-Train/Test Split
-Model Training
-Model Evaluation

# Exploratory Data Analysis (EDA)
-Checked data types and missing values
-Analyzed class imbalance
-Visualized:
-Feature distributions
-Readmission rates by age
-Correlation heatmap

# Data Preprocessing
-Label encoding for categorical variables
-Binary encoding of target variable
-Train/Test split (80/20 with stratification)

# Models Used
1. Logistic Regression
-Baseline model
-Interpretable
-Handles class imbalance with class_weight='balanced'
2. Random Forest
-Ensemble model using decision trees
-Handles non-linear relationships
-Provides feature importance

# Model Evaluation

Models were evaluated using:

-Precision
-Recall (Key metric for healthcare)
-F1-score
-ROC-AUC Score
-Confusion Matrix

# Key Insights
1. Prior hospital visits (n_inpatient) are strong predictors of readmission
2. Medication and lab activity also influence outcomes
3. Random Forest generally outperforms Logistic Regression
4. Class imbalance impacts model performance and must be handled carefully

# Technologies Used
Python
pandas
numpy
matplotlib
seaborn
scikit-learn
