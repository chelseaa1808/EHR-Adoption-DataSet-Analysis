# EHR-Adoption-DataSet-Analysis


This project explores the adoption of Electronic Health Records (EHR) in non-federal acute care hospitals using big data tools. The analysis was conducted in a PySpark environment to efficiently handle, clean, and model the dataset at scale.

**Project Overview**

*Dataset*: U.S. Department of Health & Human Services — Non-Federal Acute Care Hospital Health IT Adoption

Format: CSV

*Objective*: Analyze adoption patterns using distributed processing and machine learning in PySpark

# Workflow Summary
*Data Import & Schema Update*

Loaded CSV into Spark DataFrame

Renamed columns and updated schema types for consistency

Multimodel Imputation (PySpark MLlib + Custom Logic)

Built custom pipeline for handling missing values:

Used RandomForestRegressor and KNNImputer via PySpark integration

Performed group-based imputation (e.g., grouped by region/type)

Applied mean imputation as a fallback for remaining nulls

*Data Transformation*

Created a new Spark table after full imputation

Optimized schema for query efficiency

*SQL Queries*

Ran multiple exploratory queries via Spark SQL to derive insights:

EHR adoption by geographic region

Comparison across hospital types and sizes

Time-based adoption patterns (if applicable)

*Machine Learning Modeling*

Trained and compared multiple models (classification/regression where applicable):

Random Forest, Logistic Regression, and Gradient Boosted Trees using pyspark.ml

Evaluated model accuracy, ROC/AUC, and feature importance

*Visualization*

Used matplotlib/seaborn/plotly (outside Spark) after collecting sampled/predictive results

Visualized:

Feature importances

Adoption rate distributions

Model accuracy differences


**Tech Stack**

Apache Spark (PySpark)

Spark MLlib

Spark SQL

Python (matplotlib, seaborn, pandas for local plotting)

Jupyter Notebooks / Databricks / VS Code

Git

