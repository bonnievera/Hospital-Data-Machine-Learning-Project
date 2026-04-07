# Hospital-Data-Machine-Learning
Goal: To predict patient readmission using linear and non-parametric machine learning models.

# Project Overview

Hospital readmissions are a major challenge in healthcare, leading to increased costs and patient risk.

The goal of this project is to:

- Predict whether a patient will be readmitted (yes/no)
- Identify key factors influencing readmission
- Compare multiple machine learning models

# Key Features:
1.Patient demographics (age)
2.Hospital usage (time in hospital, inpatient visits)
3.Medical activity (lab procedures, medications)
4.Diagnosis categories
5.Diabetes-related tests (A1C, glucose)

# Machine Learning Workflow

This project follows a structured ML pipeline:

Data Loading
1. Exploratory Data Analysis (EDA)
2. Data Preprocessing
3. Feature Encoding
4. Train/Test Split
5. Model Training
6. Model Evaluation

# Exploratory Data Analysis (EDA)
1. Checked data types and missing values
2. Analyzed class imbalance
3. Visualized:
4. Feature distributions
5. Readmission rates by age
6. Correlation heatmap

# Data Preprocessing
1.Label encoding for categorical variables
2.Binary encoding of target variable
3.Train/Test split (80/20 with stratification)

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

1.Precision
2.Recall (Key metric for healthcare)
3.F1-score
4.ROC-AUC Score
5.Confusion Matrix

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
