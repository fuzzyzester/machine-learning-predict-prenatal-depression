# Predicting Prenatal Depression Using Machine Learning

## Overview
This project explores the feasibility of predicting prenatal depression using **power state data** collected from wearable devices, combined with EPDS (Edinburgh Postnatal Depression Scale) scores. By leveraging machine learning algorithms, the project aims to identify patterns in physiological and behavioral data that correlate with depressive symptoms during pregnancy.

## Objectives
- Utilize power state data to predict prenatal depression.
- Develop and evaluate machine learning models for classification.
- Provide insights into features most associated with depressive symptoms.

## Features
- **Data Preprocessing**:
  - Handled missing data using imputation and SMOTE for balancing classes.
  - Engineered features such as average daily steps, sleep duration, and inactivity periods.
- **Exploratory Data Analysis (EDA)**:
  - Conducted statistical analysis and visualized data distributions.
  - Examined correlations between features and depressive symptoms.
- **Machine Learning Pipeline**:
  - Models: Logistic Regression, Random Forest, Gradient Boosting, and Support Vector Machine (SVM).
  - Hyperparameter tuning using RandomizedSearchCV.

## Tools and Technologies
- **Programming Language**: Python
- **Libraries**: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

## Results
- **Gradient Boosting**:
  - Accuracy: 59%
  - Precision: 39%
  - Recall: 58%
  - ROC AUC: 0.54
- **Random Forest**:
  - Accuracy: 56%
  - Precision: 35%
  - Recall: 50%
  - ROC AUC: 0.58

### Key Insights
- Random Forest and Gradient Boosting demonstrated the best performance, highlighting their ability to handle complex, non-linear relationships.
- Power state data shows promise as a predictive tool for prenatal depression when combined with EPDS scores.

## Visual Highlights
### 1. **Correlation Matrix**
- Highlights relationships between features such as sleep, activity, and inactivity.
![Correlation Matrix](https://raw.githubusercontent.com/fuzzyzester/machine-learning-predict-prenatal-depression/main/screenshots/correlation-matrix.png)

### 2. **Feature Distribution**
- Visualizes the distribution of key features like daily steps and sleep duration.
![Feature Distribution](https://raw.githubusercontent.com/fuzzyzester/machine-learning-predict-prenatal-depression/main/screenshots/feature-distribution.png)

### 3. **ROC Curve**
- Compares the classification performance of all models.
![ROC Curve](https://raw.githubusercontent.com/fuzzyzester/machine-learning-predict-prenatal-depression/main/screenshots/roc-curve.png)

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/fuzzyzester/machine-learning-predict-prenatal-depression.git
