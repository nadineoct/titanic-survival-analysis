# Titanic Data Preprocessing, Feature Engineering, and Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Status](https://img.shields.io/badge/status-completed-green)
![Project](https://img.shields.io/badge/project-data--analysis-orange)
![Focus](https://img.shields.io/badge/focus-preprocessing%20%7C%20EDA%20%7C%20feature--engineering-blue)

---

## Overview

This project performs comprehensive data preprocessing, feature engineering, and exploratory data analysis (EDA) on the Titanic dataset.

The objective is to transform raw passenger data into a clean, structured, and analysis-ready dataset while extracting meaningful insights and preparing features suitable for machine learning models.

This project demonstrates key data science skills including:

- Data cleaning  
- Missing value imputation  
- Feature engineering  
- Feature scaling and standardization  
- Data visualization  
- Correlation analysis  
- Insight extraction  

## Dataset Description

The dataset contains passenger information from the Titanic disaster.

Each row represents one passenger.

### Features include:

| Feature | Description |
|---|---|
| Pclass | Passenger class (1st, 2nd, 3rd) |
| Age | Passenger age |
| Sex | Passenger gender |
| Fare | Ticket fare |
| SibSp | Number of siblings/spouses aboard |
| Parch | Number of parents/children aboard |
| Embarked | Port of embarkation |
| Survived | Survival outcome (Target variable) |

## Project Workflow

### 1. Data Exploration

Initial inspection includes:

- Dataset structure
- Missing values
- Descriptive statistics
- Feature distributions

### 2. Data Cleaning

Missing values in Age were imputed using:

Median age per passenger class (Pclass)

This method is more robust than mean imputation due to skewed age distributions.

### 3. Feature Engineering

A new feature was created:

FamilySize = SibSp + Parch + 1

This captures the total family members traveling together.

### 4. Feature Standardization

Numerical features were standardized using z-score normalization:

Z = (X − μ) / σ

This improves performance and stability for machine learning models.

Saved outputs:

- matrix.csv  
- standarazied_data.csv  

### 5. Data Visualization

Three key visualizations were created:

#### Age Distribution by Sex and Survival
File: violin_age_sex_survived.png

Shows survival patterns across age and gender.

#### Correlation Heatmap
File: correlation_heatmap.png

Shows relationships between numerical features.

#### Age vs Fare by Passenger Class
File: lmplot_age_fare_by_pclass.png

Shows interaction between socioeconomic status and survival.

## Key Insights

### 1. Women and children had higher survival priority

Children and women show significantly higher survival rates, supporting evacuation priority policies.

### 2. Passenger class strongly influenced survival

Higher-class passengers had significantly higher survival rates regardless of fare variations.

### 3. Gender and class interaction effect

Gender advantage was strongest in higher classes and weaker in lower classes.

### 4. Fare distribution is highly skewed

Log transformation helps improve numerical stability for machine learning optimization.

### 5. Correlation does not imply causation

Passenger class correlates with survival, but underlying causes include:

- Wealth
- Deck location
- Access to lifeboats

## Files in Repository

| File | Description |
|---|---|
| analysis.ipynb | Main analysis notebook |
| titanic.csv | Raw dataset |
| titanic_cleaned_engineered.csv | Cleaned dataset |
| matrix.csv | Numerical feature matrix |
| standarazied_data.csv | Standardized feature matrix |
| correlation_heatmap.png | Correlation visualization |
| violin_age_sex_survived.png | Survival distribution plot |
| lmplot_age_fare_by_pclass.png | Fare vs age visualization |
| report.md | Analysis report |

## Technologies Used

Python

Libraries:

- pandas
- numpy
- matplotlib
- seaborn

## Skills Demonstrated

Data cleaning  
Feature engineering  
Feature scaling  
Exploratory data analysis  
Data visualization  
Statistical reasoning  
Data preparation for machine learning  

## Author

Nadine Octavia

Data Science and Machine Learning Project