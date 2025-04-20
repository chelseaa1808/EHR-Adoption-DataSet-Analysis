# EHR-Adoption-DataSet-Analysis


This project focuses on analyzing the adoption of Electronic Health Records (EHR) in non-federal acute care hospitals across the U.S. Using data provided by HealthIT.gov, this repository showcases a complete pipeline from data cleaning to visualization, including machine learning-driven imputation and exploratory analysis.

Project Summary
Dataset: Non-federal acute care hospital EHR adoption data (CSV format)

Goal: Assess trends and patterns in EHR adoption using data science and machine learning techniques

Key Steps
Data Import & Schema Adjustment

Loaded CSV dataset

Renamed and standardized column schema

Dropped irrelevant columns

Data Imputation (ML & Statistical)

Performed multimodel imputation using RandomForestRegressor, KNNImputer, and others

Applied group-based imputation (e.g., by region or hospital size)

Fallback to global mean imputation for residual missing values

New Data Table Creation

Consolidated cleaned and imputed data into a new final dataset for analysis

SQL Analysis

Created multiple SQL queries to explore trends such as:

EHR adoption by region

Hospital characteristics affecting adoption

Longitudinal adoption patterns

Machine Learning Modeling

Trained and evaluated models including:

Random Forest

Logistic Regression

XGBoost

Assessed model accuracy, F1 score, and feature importance

Data Visualization

Built informative visualizations (matplotlib, seaborn, plotly) to illustrate:

Missing data before/after imputation

Model performance comparisons

EHR adoption trends and distributions

Technologies Used
Python (Pandas, NumPy, scikit-learn)

SQL 

Jupyter Notebook / VS Code

Git

