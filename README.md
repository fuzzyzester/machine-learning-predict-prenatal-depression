# **Predicting Prenatal Depression Using Machine Learning**

## **Overview**
This project investigates the potential of predicting prenatal depression using power state data collected from the Mom2B smartphone application—a research initiative by Uppsala University. By applying machine learning algorithms to wearable device data and Edinburgh Postnatal Depression Scale (EPDS) scores, this study explores early detection methods for depressive symptoms during pregnancy. The insights gained aim to support timely interventions and improve maternal mental health outcomes.

---

## **Objectives**
1. **Predict Prenatal Depression**: Utilize power state data to develop predictive models for identifying depressive symptoms during pregnancy.
2. **Model Evaluation**: Assess machine learning algorithms for accuracy, precision, recall, and overall predictive capability.
3. **Feature Insights**: Identify patterns in physiological and behavioral data correlated with depressive symptoms.

---

## **Key Features**

### **Data Preprocessing**
- **Handling Missing Data**: Missing values were addressed using imputation techniques, and class imbalance was resolved with SMOTE (Synthetic Minority Oversampling Technique).
- **Feature Engineering**: Derived key features from power state data, including:
  - Daily steps (activity levels).
  - Sleep duration (rest patterns).
  - Inactivity periods (low activity phases).

### **Exploratory Data Analysis (EDA)**
- Conducted statistical analysis and visualized feature distributions.
- Examined correlations between activity, sleep, inactivity, and EPDS scores.

### **Machine Learning Pipeline**
- **Algorithms Implemented**:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting
  - Support Vector Machine (SVM)
- **Hyperparameter Tuning**: Used `RandomizedSearchCV` for optimization.
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score, and ROC AUC.

---

## **Tools and Technologies**
- **Programming Language**: Python
- **Libraries Used**:
  - Data Processing: `pandas`, `numpy`
  - Machine Learning: `scikit-learn`
  - Visualization: `matplotlib`, `seaborn`

---

## **Results**
### **Model Performance**
| **Model**            | **Accuracy** | **Precision** | **Recall** | **ROC AUC** |
|-----------------------|--------------|---------------|------------|-------------|
| Gradient Boosting     | 59%          | 39%           | 58%        | 0.54        |
| Random Forest         | 56%          | 35%           | 50%        | 0.58        |
| Logistic Regression   | 51%          | -             | -          | 0.47        |
| Support Vector Machine| 51%          | 0.00          | 0.00       | 0.40        |

- **Gradient Boosting** and **Random Forest** performed best, demonstrating moderate success in identifying depressive symptoms.
- **Support Vector Machine** struggled to predict cases effectively.

---

## **Key Insights**
- Behavioral patterns such as activity levels and sleep duration show promise as predictive indicators of prenatal depression.
- Combining power state data with EPDS scores enhances the model's predictive capability.
- Ensemble methods like Random Forest and Gradient Boosting handle complex data relationships better than simpler models.

---


